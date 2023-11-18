# git_assignment_HeroVired
git_assignment_HeroVired - Assignment Repository created by Sunil Gaddi

QUESTION : 01 ====================================================================================================================================

Steps Followed:
1. Create a repository:
   # Assuming you're using GitHub
    git init git_assignment_HeroVired
    cd git_assignment_HeroVired
    # Create a new repository on GitHub and follow the instructions to add the remote
    git remote add origin <repository_url>
2. Create 'dev' branch and add the code:
3. Merge 'dev' branch with 'main' and release version 1:
   git checkout -b dev
    git add .
    git commit -m "Add basic calculator functionality"
    git push origin dev
    # Create a pull request on GitHub to merge 'dev' into 'main'
    # Merge the pull request on GitHub
    # Tag the release
    git tag -a v1.0 -m "Release version 1.0"
    git push origin v1.0
4. Add collaborators:
5. Create 'feature/sqrt' branch and add the 'sqrt' code:
   git checkout -b feature/sqrt
    # Add the square root feature code
    git add .
    git commit -m "Add square root feature"
    git push origin feature/sqrt
6. Bug fix in 'dev' branch:
   git checkout dev
    # Add the bug fix in the divide function
    git add .
    git commit -m "Fix divide function"
    git push origin dev
7. Create a pull request for the 'feature/sqrt' branch:
   On GitHub, create a pull request targeting the 'dev' branch.
8. Code review and improvements:
   Your team member reviews the pull request, suggests changes. Make changes locally and push again. Repeat until the code is approved.
9. Merge 'feature/sqrt' into 'dev':
    git checkout dev
    git merge feature/sqrt
    git push origin dev
10. Testing and merge into 'main', create version 2 release:
    git checkout main
    git merge dev
    # Resolve any merge conflicts if needed
    git push origin main
    # Tag the release
    git tag -a v2.0 -m "Release version 2.0"
    git push origin v2.0



QUESTION : 02 ====================================================================================================================================

Steps Followed:
1. Set up Git LFS:
   First, ensure that Git LFS is installed on your system. You can download and install it from the official Git LFS website if you haven't already.
2. Initialize a Git repository and create a branch, If you haven't already, initialize a Git repository and create a new branch 'lfs' in your repository
   # Initialize a Git repository if not already done
    git init

    # Create a branch named 'lfs'
    git checkout -b lfs
3. Configure Git LFS for your repository:
    Configure Git LFS to track files with specific extensions or files larger than a certain size. In this case, we will track files larger than 200MB
   # Configure Git LFS to track large files
    git lfs track "*.bin"  # Track binary files with the .bin extension
    git lfs track "*.zip"  # Track binary files with the .zip extension
4. Add and commit a large binary file:
    Add your large binary file(s) to the repository and commit them.
   # Add your large binary file(s)
    git add your_large_file.bin

    # Commit the file(s) using a meaningful message
    git commit -m "Add large binary file"
5. Push to the 'lfs' branch:
    Push your changes to the 'lfs' branch. Git LFS will automatically handle the large binary files.
   git push origin lfs
6. Clone the repository on another machine:
    To verify that the binary files are downloaded correctly on another machine, clone the 'lfs' branch from the 'git_assignment_HeroVired' repository.
   # Clone the repository
    git clone https://github.com/yourusername/git_assignment_HeroVired.git
    cd git_assignment_HeroVired

    # Switch to the 'lfs' branch
    git checkout lfs
7. After cloning and checking out the 'lfs' branch, the binary files should be automatically downloaded from Git LFS. You can verify this by checking the file sizes and         contents on the new machine.
8. This process will allow you to efficiently manage large binary files in your Git repository using Git LFS. Just make sure that the '.gitattributes' file contains the         correct tracking patterns for your specific binary file types.



QUESTION : 03 ====================================================================================================================================

Steps Followed:
1. Clone the GitHub repository to your local machine if you haven't already:
   git clone <repository_url>
   cd <repository_directory>
2. Create a new branch "feature/circle-area" to work on the circle area feature:
   git checkout -b feature/circle-area
3. Implement the circle area feature by editing the code in your Python file. Don't forget to uncomment the relevant code.
4. Before committing the changes, stash them to save the incomplete feature implementation:
   git stash
5. Verify that the working directory is clean:
   git status
6. Create a new branch "feature/rectangle-area" to work on the rectangle area feature:
   git checkout -b feature/rectangle-area
7. Implement the rectangle area feature by editing the code in your Python file. Don't forget to uncomment the relevant code.
8. Before committing the changes, stash them to save the incomplete feature implementation:
   git stash
9. Verify that the working directory is clean:
    git status
10. Switch back to the "feature/circle-area" branch to continue working on the circle area feature:
    git checkout feature/circle-area
11. Retrieve the stashed changes for the circle area feature:
    git stash pop
12. Complete the circle area feature implementation and save the changes, Commit the changes:
    git add .
    git commit -m "Implement circle area feature"
13. Push the changes to the repository:
    git push origin feature/circle-area
14. Switch back to the "feature/rectangle-area" branch to continue working on the rectangle area feature:
    git checkout feature/rectangle-area
15. Retrieve the stashed changes for the rectangle area feature:
    git stash pop
16. Complete the rectangle area feature implementation and save the changes.Commit the changes:
    git add .
    git commit -m "Implement rectangle area feature"
17. Push the changes to the repository:
    git push origin feature/rectangle-area
18. Create two pull requests, one for "feature/circle-area" and one for "feature/rectangle-area," targeting the "dev" branch.
19. reviewer review your pull requests.
20. After receiving approval, merge both pull requests into the "dev" or "main" branch as per your project's branching strategy.




















