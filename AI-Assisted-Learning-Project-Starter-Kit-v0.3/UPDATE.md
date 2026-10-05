# Starter Kit Update Instructions

**Document:** Update Instructions  
**Document ID:** UPDATE.md  
**Version:** 0.3  
**Status:** Starter Kit  
**Owner:** Curriculum Manager / Coordinator  
**Authority:** Starter Kit Baseline

## Purpose

Use these instructions to update an existing ChatGPT learning project to a newer
version of the AI-Assisted Learning Project Starter Kit.

The update keeps the existing ChatGPT Project and its chats. It replaces the
Starter Kit configuration used by that project.

## Update process

### 1. Update Project Instructions

Open the ChatGPT Project settings.

Replace the existing Project Instructions with the complete contents of
`PROJECT_INSTRUCTIONS.md` from the new Starter Kit release.

### 2. Delete the existing Project Source files

Remove the existing Starter Kit Project Source files from the ChatGPT Project.

ChatGPT does not currently provide an in-place replace or version operation for
Project Source files, so the old source files must be deleted before the new
source files are uploaded.

### 3. Upload the new Project Source files

Upload the Project Source files supplied by the new Starter Kit release.

These files become the project's new Starter Kit baseline.

### 4. Accept ChatGPT filename suffixes

ChatGPT may add suffixes such as `(1)` or `(2)` to filenames that have
previously been uploaded to the project, even after an earlier copy was deleted.

Do not repeatedly delete and re-upload files to try to remove these suffixes.

The `Document ID` declared inside each Markdown document is its canonical
logical identity. A suffix added by the ChatGPT upload interface does not change
that identity.

### 5. Continue using the existing project

Do not recreate the ChatGPT Project.

Existing project chats remain in place.

After the update, start or continue a chat normally. The project should use the
new Project Instructions and the newly uploaded Project Source baseline.

## Summary

The update sequence is:

```text
Update Project Instructions
        ↓
Delete old Project Source files
        ↓
Upload new Project Source files
        ↓
Continue using the existing project
```

## Scope

This procedure updates the Starter Kit configuration of an existing ChatGPT
Project.

It does not require:

- creating a new ChatGPT Project;
- recreating existing chats;
- maintaining parallel Starter Kit versions inside the project;
- repeatedly re-uploading files to remove ChatGPT-generated filename suffixes.
