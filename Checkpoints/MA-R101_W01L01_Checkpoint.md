# MA-R101_W01L01_Checkpoint: Working Loan Calculator Code Snapshot

**Course**: Integrated Math I: Algebraic Foundations & Computational Logic (GT Track)  
**Lesson**: Week 1, Lesson 1 — Algebraic Expressions & Your Rust Environment  

---

## 💻 Purpose

This checkpoint provides a working Rust code snapshot for the Loan Calculator project.  
It is designed to:  
- Help students validate their setup and compare their implementation.  
- Demonstrate how algebraic thinking translates into structured Rust programming.  
- Reinforce ARKTIK values: **Operational Mastery**, **Stewardship**, **Integrity**, and **Faith-Reason Alignment**.

Use this example to ensure your code compiles and runs successfully, and reflect on the values practiced through its creation.

---

## 💻 Code Snapshot

```rust
// ARKTIK Curriculum for Education (A.C.E.)
// Real-World Rust: Algebra in Action
// Project: Rust Loan Calculator — Powered by ARKTIK
// Course: Integrated Math I: Algebraic Foundations & Computational Logic (GT Track)

// Main Loan Calculator Program
fn main() {
    // Input Variables
    let loan_amount: f64 = 1000.0; // Loan principal
    let annual_rate: f64 = 5.0; // Annual interest rate in percentage
    let loan_term: u32 = 12; // Loan term in months

    // Calculations
    let monthly_rate = annual_rate / 12.0 / 100.0;
    let monthly_payment = loan_amount * (monthly_rate * (1.0 + monthly_rate).powf(loan_term as f64))
        / ((1.0 + monthly_rate).powf(loan_term as f64) - 1.0);

    // Output
    println!("Loan Amount: ${:.2}", loan_amount);
    println!("Annual Interest Rate: {:.2}%", annual_rate);
    println!("Loan Term: {} months", loan_term);
    println!("Monthly Payment: ${:.2}", monthly_payment);
}
```

---

## 💻 Instructions

1. **Run the Code**:  
   - Copy and paste the code into your Rust environment or IDE.  
   - Compile and run the program to verify its output.  

2. **Compare Your Code**:  
   - Check your implementation against this snapshot.  
   - Ensure your variable declarations, calculations, and output formatting align with the example.  

3. **Reflect on Key Values**:  
   - **Operational Mastery**: Did you follow the instructions carefully?  
   - **Stewardship**: Did you take responsibility for ensuring correctness in every line of code?  
   - **Integrity**: Did you debug any issues honestly and diligently?  
   - **Faith-Reason Alignment**: How does the structured logic of Rust reflect broader systems of trust and design?

4. **Test Modifications**:  
   - Modify the input variables (e.g., loan amount, interest rate, or loan term) to see how the output changes.  
   - Reflect on how small changes in input affect the larger system — a practical application of algebraic thinking.

---

## 💻 Expected Output

If the program runs successfully with the provided inputs, it should produce the following output:

```
Loan Amount: $1000.00
Annual Interest Rate: 5.00%
Loan Term: 12 months
Monthly Payment: $85.61
```

---

## 💻 Reflection Questions

1. How does this program showcase the connection between algebra and computational logic?  
2. What did you notice about the precision required in Rust programming?  
3. How does this exercise help you practice operational mastery and stewardship?

---

> _“Precision is the foundation of mastery. Stewardship transforms precision into excellence.”_  
> — ARKTIK Curriculum for Education  
