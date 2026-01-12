# Basic Preparation: Git Setup

> **Disclaimer:**  
> These notes reflect my personal understanding of Git and GitHub setup.  
> They are intended for learning purposes and do not reproduce any proprietary documentation.

---

## 1. What Is Git?

**Git** is a distributed **version control system** widely used in software development.  
It allows developers to:
- Track changes in source code
- Work on different versions of a project
- Collaborate with others efficiently
- Revert to previous states when needed

Git runs locally on your machine and does not require an internet connection to function.

---

## 2. What Is GitHub?

**GitHub** is a cloud-based platform that hosts Git repositories and provides a web interface for managing them.

With GitHub, you can:
- Store and share repositories online
- Collaborate with other developers
- Review code and manage issues
- Integrate CI/CD and automation tools

GitHub uses Git under the hood, but adds collaboration and hosting features.

---

## 3. Preparing Your Environment

Before using Git and GitHub together, you need to:

1. Install Git on your system  
2. Configure basic Git settings  
3. Authenticate with GitHub (SSH or HTTPS)

I will not include OS-specific installation steps here, since the process differs depending on your operating system.

---

## 4. Installing Git

Official installation guides:

- Git Guides – Install Git  
  https://github.com/git-guides/install-git

- Git Book – Installing Git from Source  
  https://git-scm.com/book/en/v2/Getting-Started-Installing-Git

---

## 5. Basic Git Configuration

After installation, Git requires minimal setup (username, email, etc.).

Official tutorial:
- Git Tutorial  
  https://git-scm.com/docs/gittutorial

---

## 6. GitHub Authentication (SSH)

GitHub supports multiple authentication methods.  
In my setup, I chose **SSH authentication**, but HTTPS is also a valid option.

### Why SSH?
- No need to enter credentials on every push
- More secure for long-term use
- Commonly used in professional environments

GitHub SSH documentation:

- Connecting to GitHub with SSH  
  https://docs.github.com/en/authentication/connecting-to-github-with-ssh

- Using SSH Agent Forwarding  
  https://docs.github.com/en/authentication/connecting-to-github-with-ssh/using-ssh-agent-forwarding

---

## References

The following resources were used as **learning references** for Git and GitHub setup:

- Git Official Documentation  
  https://git-scm.com

- GitHub Docs  
  https://docs.github.com

---

## Final Notes

Git is a foundational tool for modern software development.  
Setting it up early and understanding its basics is essential for collaboration, version control, and professional workflows.