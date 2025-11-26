# Modeler - Product Backlog

## High Priority

### Add "Reset to Home" Keybind

**Description:**
Implement a keyboard shortcut that instantly returns the camera/player position to the initial "home" location in the 3D world. This allows users to quickly reorient themselves after navigating deep into the repository structure.

**Rationale:**
Users exploring large codebases can easily get disoriented or lost in the 3D space. A quick way to return to the starting position improves navigation UX and reduces frustration.

**Acceptance Criteria:**
- [ ] Pressing a designated key (e.g., `H` or `Home`) resets the camera position to the initial spawn point
- [ ] Pressing the key also resets the camera rotation to the default viewing angle
- [ ] The reset action is smooth (animated transition vs instant teleport - TBD)
- [ ] The keybind is documented in the README.md Controls section
- [ ] The keybind is displayed in the UI (either in a help overlay or controls panel)
- [ ] The home position is configurable/rememberable (can be set by user - optional enhancement)
- [ ] Works consistently across all navigation states (whether cursor is locked or unlocked)

**Technical Notes:**
- Update camera position and rotation in the camera controller
- Consider adding a brief animation/transition (e.g., 500ms smooth interpolation)
- Default home position should be the initial camera spawn location (likely centered view of root directory)
- May need to store the initial camera state when WorldBuilder first creates the scene

**Priority:** High
**Effort:** Small (1-2 hours)
**Dependencies:** None

---

## Medium Priority

(Add future backlog items here)

---

## Low Priority / Future Ideas

(Add future backlog items here)
