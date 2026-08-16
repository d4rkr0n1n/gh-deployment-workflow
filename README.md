# GitHub Pages Deployment

## About the project
The goal of this project is to help me learn the notion of continuous integration and continuous deployment. I wrote a simple GitHub Actions workflow to deploy a static website to GitHub Pages.
I wrote a GitHub action file ``deploy.yml`` that deploys any changes made to the index.html file to GitHub Pages. It should only deploy the file when the ``index.html`` file is changed.

## Repotree
```
├── .github
│   └── workflows
│       └── deploy.yml
├── .gitignore
├── index.html
└── README.md
```

## Specification
1. Automatically deploy `index.html` changes to GitHub Pages when pushed to `main` branch
2. Trigger workflow only when `index.html` file is modified (path filter)
3. Checkout repository, build artifacts, and deploy to `gh-pages` branch
4. Deployment should complete within 2-3 minutes with clear success/failure feedback
5. Site goes live automatically after successful deployment to GitHub Pages

## Project URL: https://roadmap.sh/projects/github-actions-deployment-workflow
