# CI/CD 

> Mini‑Project Roadmap:
> 
> Welcome to the CI/CD mini‑project! Follow the steps below to build and deploy your own pipeline.

---

## 📚 Core Resources to Revise

### Continuous Integration (CI)
1. **YouTube – GitHub Actions CI for Beginners**
   https://www.youtube.com/watch?v=R8_veQiYBjI
2. **Website – GitLab CI/CD Basics**
   https://about.gitlab.com/topics/ci-cd/
3. **YouTube – Jenkins Introduction**
   - Link 1: https://www.youtube.com/watch?v=cy2257Y7I54
   - Link 2: https://www.lambdatest.com/blog/jenkins-pipeline-tutorial/

### Continuous Deployment (CD)
1. **YouTube – Deploy Static Site with GitHub Actions**
   https://www.youtube.com/watch?v=sT_zXIX3ZA0
2. **Website – Deploying to Vercel & Netlify**
   - Link 1: https://www.youtube.com/watch?v=sMj3HFIfhLI
   - Link 2: https://www.netlify.com/blog/2016/09/29/a-step-by-step-guide-deploying-on-netlify/
3. **YouTube – Docker CI/CD Pipeline Demo**
   https://www.youtube.com/watch?v=ylEy4eLdhFs

---

## 🗺️ Roadmap & Tasks

### 1. Learn CI/CD Fundamentals
- Read or watch any of the CI resources to understand:
- **What** CI/CD means
- **Why** it matters (code quality, faster releases)
- **Who** uses it and in **which** scenarios

### 2. Set Up Your CI Pipeline
- In a GitHub (or GitLab) repo, create a **CI workflow** that:
- Runs your project’s tests or lint checks on each push/PR
- Fails visibly if something breaks
- Experiment with **GitHub Actions**, **GitLab CI**, or **Jenkins**

### 3. Extend to Deployment (CD)
- Choose one deployment target:
- **Static website** → GitHub Pages, Netlify or Vercel
- **Docker container** → build & push to Docker Hub or GitHub Container Registry
- Update your workflow so that **after** successful CI, it:
- **Deploys** your app automatically

### 4. Explore Advanced Tools (Optional)
- Investigate how **AWS CodePipeline**, **CodeBuild**, and **CodeDeploy** fit into more complex CD flows
- Deep‑dive into branching strategies (GitFlow, trunk‑based) and workflow gates

---

## 📝 Mini‑Project Submission

1. **Repo Setup**

2. Host a simple app or static site in a GitHub/GitLab repo.

3. **CI Workflow:** Add a file at `.github/workflows/ci.yml` (or equivalent) that runs tests/lint.

4. **CD Workflow: ** Add a file at `.github/workflows/cd.yml` (or in the same workflow) that deploys on success.

5. **Documentation:** In your `README.md`, include:
- A brief description of your **CI steps**
- Which **CD target** you chose and the commands used

6. **Submit**
- 🔗 Your repo URL
- ✏️ A small summary of how your pipeline works

---

_By completing these tasks, you’ll have built and deployed your own CI/CD pipeline—an invaluable addition to your CV! 🚀_