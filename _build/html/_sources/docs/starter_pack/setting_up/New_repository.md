# Create a new repository

**Step 1**: Go to your GitHub account home page. There is a 'New' button near the left handside top corner as per below picture.

![new_repository_step1](./new_repository_step1.png)


**Step 2**: After clicking 'New' button, key in your repository name.
Click certain setting as per your situation.

![new_repository_step2](./new_repository_step2.png)

**Step 3**: Add repository via terminal window. In this example, the repository calls 'AMAAI'.

```bash
git add AMAAI
```
Alternative use 'git add .' to represent *add all* the unpushed file.
```bash
git add .
```

**Step 4**: Add descriotion for your repository. Remember to use '*TEXT*' for text content.

```bash
git commit -m 'description of this committed file'
```

**Step 5 (optional)**: Use 'git branch' to find current branch name.

```bash 
git branch
```
![new_repository_step5](./new_repository_step5.png)



**Step 6**: Update repository to GitHub. In this example, the branch name calls 'main'.

```bash
git push origin main
```

**Step 7**: 




