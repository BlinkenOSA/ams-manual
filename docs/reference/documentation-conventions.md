# Documentation conventions

This manual uses the following conventions:

- **Bold text** names a label, button, menu item, tab, or other interface element.
- `Monospace text` shows an exact value, format, identifier, or technical name.
- Numbered lists describe procedures that should be followed in order.
- Notes add context; warnings identify a risk to data, access, or policy compliance.

## Source and verification status

The initial manual was derived from the AMS navigation, route access configuration, tables, and form definitions. It describes the current interface but does not infer institutional policy that is absent from the application.

When updating a page:

1. Verify labels and available actions against the current AMS interface.
2. Test the procedure with an account that has the documented role.
3. Separate software behavior from institutional policy.
4. Add a screenshot only when it clarifies a decision or multi-step action.
5. Avoid real personal, confidential, or restricted data in examples.

## Editorial style

Use **AMS** after the first occurrence of **Archival Management System**. Address the reader as “you,” use direct verbs, and keep one task per procedure. Prefer the terms used in the interface even when a local synonym is common.

## Standard module-page structure

Use the following structure when a module has both a record list and a record form:

1. **[Module] List**
    1. **Filters** — describe every filter and how filters combine.
    2. **Columns** — explain each displayed value and mark whether the column is sortable.
    3. **Row actions** — explain each action and its side effects.
    4. **Footer action** — explain New and any other actions below the table.
2. **[Module] Form**
    1. Explain View, Create, and Edit behavior where applicable.
    2. State prerequisites before the field reference.
    3. List each field with its requirement, input type or source, and guidance.
    4. Cross-link reusable controls to [Special form fields](../getting-started/special-form-fields.md).

Avoid repeating a separate creation procedure when selecting **New** simply opens the form already documented on the page. Describe legacy fields in the field reference and maintenance behavior with the corresponding list or form action.
