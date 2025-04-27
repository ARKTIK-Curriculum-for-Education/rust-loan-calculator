# Repository Setup Guide: Rust Loan Calculator

Welcome to the **Rust Loan Calculator** repository! This guide will help you set up and work with this project effectively, whether you're an instructor, student, or contributor.

---

## Repository Overview
- **Repository URL**: [Rust Loan Calculator](https://github.com/ARKTIK-Curriculum-for-Education/rust-loan-calculator)
- **Description**:  
  Proof of Concept for the **A.C.E. Lesson Meta**:  
  - **Course Name**: Integrated Math I: Algebraic Foundations & Computational Logic (GT Track)  
  - **Code**: ACE-MA-R101-GT  
  - **Week/Lesson**: W01/L01  
  - **Subject Area**: Mathematics & Computational Thinking  
  - **Execution Time**: 90–120 min  

This repository is designed to support students in grades 6–12 and educators in computational thinking and mathematical concepts using Rust programming.

---

## Step 1: Fork the Repository
1. Navigate to the repository page: [Rust Loan Calculator](https://github.com/ARKTIK-Curriculum-for-Education/rust-loan-calculator).
2. Click the **Fork** button in the top-right corner to create your own copy of the repository.

---

## Step 2: Clone the Repository
1. Go to your forked repository.
2. Click the **Code** button and copy the HTTPS, SSH, or GitHub CLI URL.  
   For example (HTTPS):  
   ```bash
   https://github.com/<your-username>/rust-loan-calculator.git
   ```
3. Open a terminal on your local machine and run the following command:
   ```bash
   git clone <copied-url>
   ```
4. Navigate into the cloned directory:
   ```bash
   cd rust-loan-calculator
   ```

---

## Step 3: Install Prerequisites
Ensure the following tools are installed on your system:
- [Rust](https://www.rust-lang.org/tools/install): The Rust programming language.
- [Cargo](https://doc.rust-lang.org/cargo/): Rust's package manager.
- [Git](https://git-scm.com/): Version control system.

Verify your installations:
```bash
rustc --version   # Ensure Rust is installed
cargo --version   # Ensure Cargo is installed
git --version     # Ensure Git is installed
```

---

## Step 4: Pull Latest Changes from Upstream
Keep your forked repository up-to-date with the original repository:
1. Add the original repository as an upstream remote:
   ```bash
   git remote add upstream https://github.com/ARKTIK-Curriculum-for-Education/rust-loan-calculator.git
   ```
2. Fetch changes from upstream:
   ```bash
   git fetch upstream
   ```
3. Merge updates into your local `main` branch:
   ```bash
   git checkout main
   git merge upstream/main
   ```

---

## Step 5: Workflow for Making Changes
1. **Create a New Branch**:  
   Use a descriptive branch name for your changes:
   ```bash
   git checkout -b feature/<your-branch-name>
   ```
2. **Make Changes**:  
   Edit the code or documentation as needed using your preferred IDE or text editor.
3. **Test Your Changes**:  
   Run the following command to ensure your changes work correctly:
   ```bash
   cargo test
   ```
4. **Commit Your Changes**:  
   Stage and commit your changes with a meaningful message:
   ```bash
   git add .
   git commit -m "Describe your changes"
   ```
5. **Push Your Branch**:  
   Push your branch to your forked repository:
   ```bash
   git push origin feature/<your-branch-name>
   ```

---

## Step 6: Submit a Pull Request
1. Navigate to your forked repository on GitHub.
2. Click **Compare & pull request**.
3. Add a detailed description of your changes and submit the pull request.
4. Wait for feedback or approval from the maintainers.

---

## Troubleshooting
### Common Issues
- **Permission Denied (SSH)**:
  - Ensure your SSH key is added to your GitHub account.
  - Follow GitHub's [SSH key setup guide](https://docs.github.com/en/authentication/connecting-to-github-with-ssh).
- **Dependency Errors**:
  - Run `cargo update` to update dependencies.
  - Check the [Rust documentation](https://doc.rust-lang.org/) for further help.

---

## Additional Resources
- [Rust Official Documentation](https://doc.rust-lang.org/)
- [GitHub Help](https://docs.github.com/)
- [Rust Loan Calculator Repository](https://github.com/ARKTIK-Curriculum-for-Education/rust-loan-calculator)

---

> _“This repository empowers operational mastery and computational thinking through real-world systems building.”_  
> — ARKTIK Curriculum for Education

---

Let me know if you'd like further adjustments or help publishing this guide!
