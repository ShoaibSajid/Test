This is a test Repo

# heading 1
## heading 2

## Git Branch Operations Diagram

```mermaid
gitgraph
    commit id: "Initial commit"
    branch feature-a
    checkout feature-a
    commit id: "Feature A commit 1"
    commit id: "Feature A commit 2"
    checkout main
    merge feature-a
    commit id: "Hotfix commit"
    branch feature-b
    checkout feature-b
    commit id: "Feature B commit 1"
    checkout main
    commit id: "Main commit"
    checkout feature-b
    commit id: "Feature B commit 2"
    checkout main
    merge feature-b
    commit id: "Release commit"
    branch feature-c
    checkout feature-c
    commit id: "Feature C commit 1"
    commit id: "Feature C commit 2"
    checkout main
    commit id: "Main commit 2"
    checkout feature-c
    rebase main
    checkout main
    merge feature-c
```

### Git Operations Explained

1. **Initial commit**: Starting point of the repository
2. **Feature branches**: Separate branches for developing new features
3. **Checkout**: Switching between branches
4. **Merge**: Combining feature branch changes into main branch
5. **Rebase**: Moving feature branch commits on top of main branch
6. **Hotfix**: Quick fixes made directly on main branch

**Common Git Workflow:**
- Create feature branches from main
- Develop features in isolation
- Merge or rebase feature branches back to main
- Handle hotfixes and releases on main branch