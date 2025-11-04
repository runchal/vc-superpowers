# Known Issues

## tsx Command Not Found Error (SessionStart Hook)

**Status**: Open
**Severity**: Low (cosmetic only - doesn't affect plugin functionality)

**Symptoms**:
```
SessionStart:startup says: Plugin hook error: sh: tsx: command not found
```

**Impact**:
- Error message appears at session start
- Does NOT prevent plugin from working
- All `/vc:` and `/vc2:` commands work normally

**Root Cause**:
- Session-start hook was removed but error persists
- May be cached or there's another hook triggering this
- Need to investigate plugin.json or other hook configurations

**Workaround**:
- Ignore the error - plugin works fine
- Commands load and execute normally

**Next Steps to Fix**:
1. Check if plugin.json needs explicit "hooks": null
2. Investigate if there's a hooks cache that needs clearing
3. Compare with working plugins (superpowers, episodic-memory)
4. May need to clear Claude Code cache completely

**Date Reported**: 2025-11-03
**Reporter**: Amit Runchal
