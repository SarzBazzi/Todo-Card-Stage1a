# Todo-Card-Stage1a
Stage 1a assignment of HNG14 internship

# Todo Card – Stage 1 vs Stage 0

## What Changed

* Introduced **state management (`currentTodo`)** instead of static content
* Added **edit mode** (update title, description, priority, due date)
* Implemented **expand/collapse description**
* Added **interactive status controls** (Pending / In Progress / Done)
* Improved **time handling** (detailed countdown + overdue indicator)
* Replaced alerts with **toast notifications**
* Enhanced **delete flow** with animation + feedback
* Made **priority fully dynamic** (badge, indicator, accent bar)
* Modular **render functions** for consistent UI updates

---

## New Design Decisions

* **State-driven UI** (data → UI rendering)
* **Separation of concerns** (state, render, events)
* **Inline editing** instead of modal
* **Non-blocking feedback** (toasts over alerts)
* Built with **testability + scalability in mind**

---

## Known Limitations

* No data persistence (resets on reload)
* Single todo only (not reusable list yet)
* Minimal form validation
* Basic timezone handling
* Not optimized for large-scale usage

---

## Accessibility Notes

**Improvements**

* Uses `aria-expanded`, `aria-controls`
* `aria-live` for time updates
* Better focus handling in edit mode

**Gaps**

* Toasts not screen-reader friendly
* Status changes not fully announced
* Some buttons rely heavily on visuals

---

## Summary

Stage 1 upgrades the card from a **static demo → interactive, state-driven component** ready for scaling into a full app.
