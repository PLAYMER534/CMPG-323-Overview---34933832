# CMPG-323-Overview---34933832

# Branching Approach 
A clearly defined branching approach promotes cooperation, guarantees code quality, and aids in process management. In the CMPG 323 module, we will apply the Gitflow branching technique to every project. The following categories of branches are included in this strategy:

Main Branch (main): 

The production branch is this. The code that is either in production or ready for release may be found on the main branch.
Create a Branch (develop):

This branch acts as a feature integration branch. This branch will contain all features that have been finished and tested.
Branches of Features (feature/*):

The purpose of these branches is to build improved or additional functionality.
naming guidelines: characteristic/feature-name
Diverge from: cultivate
Reintegrate into: create
Feature/add-login-functionality, for instance
Branches for releases (release/*):

The preparation for a fresh production release is supported by these branches.
naming guidelines:version/release number
Diverge from: cultivate
Combine into: grow and primary
For instance, release/1.0.0
Branches for Hotfixes (hotfix/*):

These branches are intended to swiftly fix serious issues with the code that is in production.
Name convention: description of the hotfix or problem
Diverge from the primary
Reintegrate into: main and advance
For instance, hotfix/fix-login-bug

# Use of .gitignore file
The .gitignore file specifies which files and directories to ignore in a project, ensuring that sensitive and irrelevant files do not get committed to the repository. Here is an explanation of its usage within each project:

Purpose:

Prevents sensitive information (like API keys, passwords) and system-specific files (like OS-generated files) from being committed.
Reduces repository clutter by ignoring files that do not need to be tracked (like build artifacts, log files).

# Storage of Credentials and Sensitive Information
Maintaining the confidentiality and integrity of your projects depends on securely storing login credentials and sensitive data. The following are guidelines for managing sensitive data:

Environmental Factors:

Environment variables are a good place to keep private data, such as passwords and API credentials.
To handle environment variables, use a library or package (e.g., dotenv for Python or Node.js).
Management of Secrets:

To store and manage secrets, use the secret management tools offered by cloud services (such as Azure Key Vault and AWS Secrets Manager).
Files for configuration:

Keep sensitive information-containing configuration files off of the repository.
If configuration files must be versioned, avoid explicitly include sensitive data. Make use of environment variables instead.
