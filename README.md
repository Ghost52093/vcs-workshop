# Version Control Systems Workshop

A comprehensive one-day workshop covering the evolution and practical usage of version control systems from CVS to modern distributed systems.

## Overview

This repository contains a complete tutorial and hands-on workshop materials for understanding version control systems (VCS), their evolution, and practical migration strategies. The workshop covers four major VCS platforms with deep technical dives and practical exercises.

## Workshop Contents

### Systems Covered

- **CVS** (Concurrent Versions System) - Historical foundation and legacy systems
- **Subversion (SVN)** - Centralized version control evolution
- **Git** - The distributed revolution and current industry standard
- **Mercurial (Hg)** - Alternative distributed approach with focus on simplicity

### Key Features

- 📚 **Comprehensive Tutorial**: Full-day structured learning path (8 hours)
- 🔧 **Hands-On Exercises**: Practical examples for each VCS
- 📊 **Comparison Matrices**: Detailed feature and performance comparisons
- 🔄 **Migration Guides**: Step-by-step migration strategies between systems
- 📖 **Org-Mode Format**: Complete tutorial in Emacs org-mode for easy navigation
- 🚀 **Modern Context**: Including emerging alternatives like Jujutsu, Pijul, and Fossil

## Quick Start

### Prerequisites

```bash
# Ubuntu/Debian
sudo apt-get update
sudo apt-get install -y cvs subversion git mercurial

# macOS
brew install cvs subversion git mercurial

# Verify installations
cvs --version && svn --version && git --version && hg --version
```

### Workshop Structure

```
vcs-workshop/
├── vcs-tutorial.org    # Complete tutorial in org-mode
├── README.md           # This file
└── exercises/          # Hands-on exercise files (created during workshop)
    ├── cvs/
    ├── svn/
    ├── git/
    └── hg/
```

## Tutorial Sections

1. **Introduction & Setup** (30 min)
   - VCS fundamentals
   - Evolution timeline
   - Environment setup

2. **CVS Deep Dive** (60 min)
   - Architecture and concepts
   - Hands-on exercises
   - Limitations analysis

3. **Subversion Mastery** (75 min)
   - Improvements over CVS
   - Branching and merging
   - Properties and metadata

4. **Git Revolution** (90 min)
   - Distributed model
   - Advanced workflows
   - Internals exploration

5. **Mercurial Alternative** (60 min)
   - Philosophy differences
   - Phases and bookmarks
   - Extension system

6. **Comparative Analysis** (45 min)
   - Feature matrices
   - Performance benchmarks
   - Migration strategies

7. **Modern Landscape** (30 min)
   - Current market share
   - Emerging alternatives
   - Best practices

## Key Learning Outcomes

After completing this workshop, you will:

- ✅ Understand the evolution from centralized to distributed VCS
- ✅ Master basic and advanced operations in all four systems
- ✅ Know how to migrate repositories between different VCS
- ✅ Make informed decisions about VCS selection for projects
- ✅ Apply best practices for version control in any system

## Who Should Attend

- 👨‍💻 Software developers wanting to understand VCS deeply
- 🏗️ DevOps engineers managing diverse VCS infrastructure
- 📚 Technical leads making tooling decisions
- 🔄 Teams planning VCS migrations
- 🎓 Students learning software engineering practices

## Using the Tutorial

### For Emacs Users

```bash
emacs vcs-tutorial.org
```

Navigate with:
- `TAB` - Expand/collapse sections
- `Shift-TAB` - Cycle visibility
- `C-c C-n/p` - Next/previous heading
- `C-c C-x C-v` - Toggle inline images

### For Other Editors

The org file is plain text and readable in any editor. For best experience:
- VS Code: Install "Org Mode" extension
- Vim: Use vim-orgmode plugin
- Online: Use GitHub's org-mode rendering

## Migration Quick Reference

### CVS → SVN
```bash
cvs2svn --svnrepos /new/svn/repo /old/cvs/repo
```

### SVN → Git
```bash
git svn clone --stdlayout http://svn.example.com/repo
```

### Git → Mercurial
```bash
hg clone git+ssh://git@github.com/user/repo.git
```

### Mercurial → Git
```bash
hg-fast-export.sh -r . | git fast-import
```

## Additional Resources

- 📖 [Pro Git Book](https://git-scm.com/book)
- 📖 [SVN Red Bean Book](http://svnbook.red-bean.com/)
- 📖 [Mercurial Guide](https://www.mercurial-scm.org/guide)
- 🎮 [Learn Git Branching](https://learngitbranching.js.org/)
- 🔧 [Git GUI Clients](https://git-scm.com/downloads/guis)

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request with:
- Additional exercises
- Migration examples
- Tool recommendations
- Corrections or clarifications

## License

This workshop material is provided under the MIT License. See LICENSE file for details.

## Authors

- Workshop materials developed for comprehensive VCS education
- Contributions welcome from the community

## Acknowledgments

Special thanks to:
- Linus Torvalds for Git
- CollabNet for Subversion
- Matt Mackall for Mercurial
- The open source community for continuous VCS innovation

---

**Ready to master version control?** Open `vcs-tutorial.org` and begin your journey through VCS history and modern practices!