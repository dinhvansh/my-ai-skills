# E-Office Documentation Cleanup Example

This example shows how to use the `project-documentation-cleanup` skill for an internal e-office, document management, approval, or e-signature project.

## Recommended Prompt

```md
Use the project-documentation-cleanup skill.

This is an internal e-office / document signing system. Please scan the current repository and clean up all Markdown documentation.

Requirements:

1. Treat source code as the source of truth.
2. Do not delete old Markdown files permanently.
3. Classify all `.md` files into core, draft, outdated, duplicate, reference, or unknown.
4. Create `docs/DOCUMENTATION_AUDIT_REPORT.md` before modifying documentation.
5. Archive non-core documents under `docs/archive`.
6. Rewrite the final documentation set:
   - README.md
   - docs/DOCS_INDEX.md
   - docs/01_PROJECT_OVERVIEW.md
   - docs/02_SYSTEM_ARCHITECTURE.md
   - docs/03_BUSINESS_WORKFLOW.md
   - docs/04_PERMISSION_MODEL.md
   - docs/05_DOCUMENT_TYPE_CONFIG.md
   - docs/06_E_SIGNATURE_FLOW.md
   - docs/07_DATABASE_SCHEMA.md
   - docs/08_API_DOCUMENTATION.md
   - docs/09_FRONTEND_STRUCTURE.md
   - docs/10_BACKEND_STRUCTURE.md
   - docs/11_DEPLOYMENT_GUIDE.md
   - docs/12_SECURITY_REVIEW.md
   - docs/13_TESTING_GUIDE.md
   - docs/14_CHANGELOG.md
   - docs/15_ROADMAP.md

Pay special attention to:

- Document creation flow
- Document type configuration
- Auto-numbering rules
- Approval requirement
- Default security level
- Default visibility scope
- Department-based visibility
- Role-based permissions
- E-signature flow
- PDF signature field coordinate system
- Audit logs
- Legal/security notes

Do not invent features. If something is unclear, write `TODO: Verify with source owner`.
```

## Important Review Areas For E-Office Projects

| Area | Why It Matters |
|---|---|
| Permission model | Prevents users from viewing or editing unauthorized documents |
| Document type configuration | Controls default approval, signing, numbering, and visibility rules |
| Approval flow | Determines who can approve and when a document moves to the next status |
| E-signature flow | Affects legal validity, auditability, and user trust |
| PDF coordinate system | Prevents signature fields from being misplaced in the final PDF |
| Audit log | Supports traceability and compliance review |
| Security review | Reduces risk around file access, roles, secrets, and document visibility |

## Suggested Final Docs

```txt
README.md
docs/
  DOCS_INDEX.md
  01_PROJECT_OVERVIEW.md
  02_SYSTEM_ARCHITECTURE.md
  03_BUSINESS_WORKFLOW.md
  04_PERMISSION_MODEL.md
  05_DOCUMENT_TYPE_CONFIG.md
  06_E_SIGNATURE_FLOW.md
  07_DATABASE_SCHEMA.md
  08_API_DOCUMENTATION.md
  09_FRONTEND_STRUCTURE.md
  10_BACKEND_STRUCTURE.md
  11_DEPLOYMENT_GUIDE.md
  12_SECURITY_REVIEW.md
  13_TESTING_GUIDE.md
  14_CHANGELOG.md
  15_ROADMAP.md
```

## Minimal Trigger Prompt

```md
Use the project-documentation-cleanup skill for this e-office project. Clean up all Markdown files, create an audit report, archive old docs, and rewrite the final documentation set based on the current codebase.
```
