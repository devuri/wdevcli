# Support

## Getting Help

### Self-Help Resources (Start Here)
- **[Documentation](https://docs.wdevcli.com)** - Complete guides and CLI reference
- **[FAQ](https://docs.wdevcli.com/faq)** - Common questions and solutions
- **[Troubleshooting](https://docs.wdevcli.com/faq#troubleshooting)** - Fix common issues

### Built-in Help
```bash
wdev --help           # Show all commands
wdev examples         # Usage examples
wdev doctor           # Health diagnostics
wdev <command> --help # Command-specific help
```

## Community Support

**[GitHub Issues](https://github.com/devuri/wdev-community/issues)**
- Bug reports
- Feature requests  
- General questions
- Community discussion

**Please search existing issues first** - your question might already be answered.

## Direct Support

**Email:** support@wdevcli.com

Use email for:
- License and billing questions
- Installation problems
- Private technical issues

## When Reporting Issues

Include this information to help us help you:

### System Info
```bash
wdev doctor --json    # System diagnostics
wdev --version        # WDev version
docker --version      # Docker version
```

### Problem Details
- What you were trying to do
- What happened instead
- Error messages (exact text)
- Steps to reproduce

### Example Issue Report
```
**Problem:** Site won't start after cloning

**System:** 
- WDev: v0.19.2
- OS: macOS 13.2
- Docker: 24.0.1

**Steps:**
1. wdev pull example.com --token ABC123
2. wdev start example

**Error:** 
Container failed to start: port already in use

**Expected:** Site should start at https://example.test
```

## Response Times

We'll get back to you as soon as we can. Response times depend on:
- **Issue complexity**
- **Current support volume** 
- **License type** (paid licenses get priority)

## What We Can Help With

✅ **Installation and setup**  
✅ **Using WDev features**  
✅ **Troubleshooting errors**  
✅ **License questions**  
✅ **Bug reports**  

❌ **Custom development work**  
❌ **WordPress-specific issues unrelated to WDev**  
❌ **General Docker or system administration**  
❌ **Third-party plugin problems**  

## Before Contacting Support

1. **Check the docs** - Most questions are answered there
2. **Try `wdev doctor`** - Identifies common problems
3. **Search GitHub issues** - Someone may have had the same problem
4. **Include system info** - Helps us help you faster


**Support provided for WDev v0.19.2 and later**
