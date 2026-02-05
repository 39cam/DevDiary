# Git: Commits  

A well-structured commit makes it easier for you and other developers to understand what changes were made and the reasoning behind them. This is particularly helpful when debugging or reviewing past work.  

Additionally, good commit messages are useful when you return to a project after some time away. It’s easy to forget why certain decisions were made, and descriptive commits act as a record of your thought process.  

A strong commit message should explain *why* a change was made, not just what was changed. In other words, it should describe the problem you were solving and how your update addressed it.  

## Commit Subject  

The subject is a short summary of the change you made to the project.  

### Character limit  

GitHub allows up to 72 characters for the commit subject, so it’s best to keep your summary within this limit.  

## Commit Body  

The body provides a brief but clear explanation of what you did.  

It should describe the problem you were addressing and how your changes solve it.  

### Example  

Subject:  
Add missing link and alt text to the company logo  

Body:  
Screen readers cannot properly describe images to users with visual impairments without this information.  

This type of commit is useful because it:  

- Clearly states what action was taken in the subject.  
- Explains *why* the change was necessary in the body.  
- Separates the subject and body with a blank line, which is a common best practice for readability.  

Different teams may have their own specific commit conventions, but the general principles remain the same.  

## When to commit  

You can think of a commit as a snapshot of your project at a specific moment in time. Each commit saves the current state of your code, allowing you to review or restore it later if needed.  

A good practice is to commit whenever you make a meaningful change. This creates a clear history of your progress and makes your workflow easier to follow.  

For example, you should consider making a commit when you:  

- Finish a feature that works as expected  
- Fix a bug  
- Correct a typo or small issue  

At some point, you may complete something that finally works perfectly — that’s a great moment to commit. If it breaks later and you’re unsure what changed, you can look back through your commit history, revert to a previous working version, or analyze what your code looked like at that time.