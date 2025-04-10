# DMS.Demo.Git.Branching.GitHubFlow.MergePR.Bad02
Steps taken to replicate:
1. Create a new class library project.
2. Add project to source control.
3. Create feature branch named 'feature/foo' & checkout.
4. Add a new class named 'Class2.cs'.
5. Add a comment to 'Class2.cs' : '// Branch: feature/foo | Commit #1'.
6. Commit changes: 'Branch: feature/foo | Commit #1'.
7. Checkout branch 'master'.
8. Add a comment to 'Class1.cs' : '// Branch: master | Commit #2'
9. Commit changes: 'Branch: master | Commit #2'.
10. Add a comment to 'Class1.cs' : '// Branch: master | Commit #3'
11. Commit changes: 'Branch: master | Commit #3'.
12. Checkout branch 'feature/foo'.
13. Merge branch 'master' into 'feature/foo'.
14. Add a comment to 'Class2.cs' : '// Branch: feature/foo | Commit #4'
15. Commit changes: 'Branch: feature/foo | Commit #4'.
16. Add a comment to 'Class2.cs' : '// Branch: feature/foo | Commit #5'
17. Commit changes: 'Branch: feature/foo | Commit #5'.
18. Create a PR branch from 'master' named 'pull/2/merge' & checkout.
19. Merge branch 'feature/foo' into 'pull/2/merge'.
20. Push branches 'master' & 'pull/2/merge'.
21. Create a new pull request. Merge Into: 'master' | From: 'pull/2/merge'
22. Merge pull request.
23. Checkout branch 'master'.
24. Pull latest changes.
25. Evaluate commit history/line.

![image](https://github.com/user-attachments/assets/48d5d6eb-3998-4b55-bcc6-f8c5656a357e)