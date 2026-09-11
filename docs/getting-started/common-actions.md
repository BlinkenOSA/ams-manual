# Common actions

AMS uses the same interaction patterns across most modules.

## Tables

Tables display lists of records. Most module landing pages use a table to help you find a record and choose what to do with it.

If a table contains more records than fit on one page, use the pagination controls below it to move between pages, jump to a specific page, or change the number of records shown per page. Select a sortable column heading to change the order.

When filters are available, they appear above the table. Filters can include text search, controlled-value selectors, date shortcuts, or archival-hierarchy selections. Clear active filters if an expected record is missing.

Each row can have action buttons. The most common actions are:

- <span class="ams-ui-button ams-ui-button--small" aria-hidden="true"><svg viewBox="64 64 896 896" focusable="false"><path d="M942.2 486.2C847.4 286.5 704.1 186 512 186c-192.2 0-335.4 100.5-430.2 300.3a60.3 60.3 0 000 51.5C176.6 737.5 319.9 838 512 838c192.2 0 335.4-100.5 430.2-300.3 7.7-16.2 7.7-35 0-51.5zM512 766c-161.3 0-279.4-81.8-362.7-254C232.6 339.8 350.7 258 512 258c161.3 0 279.4 81.8 362.7 254C791.5 684.2 673.4 766 512 766zm-4-430c-97.2 0-176 78.8-176 176s78.8 176 176 176 176-78.8 176-176-78.8-176-176-176zm0 288c-61.9 0-112-50.1-112-112s50.1-112 112-112 112 50.1 112 112-50.1 112-112 112z"></path></svg></span> **View** — open the record without allowing changes;
- <span class="ams-ui-button ams-ui-button--small" aria-hidden="true"><svg viewBox="64 64 896 896" focusable="false"><path d="M257.7 752c2 0 4-.2 6-.5L431.9 722c2-.4 3.9-1.3 5.3-2.8l423.9-423.9a9.96 9.96 0 000-14.1L694.9 114.9c-1.9-1.9-4.4-2.9-7.1-2.9s-5.2 1-7.1 2.9L256.8 538.8c-1.5 1.5-2.4 3.3-2.8 5.3l-29.5 168.2a33.5 33.5 0 009.4 29.8c6.6 6.4 14.9 9.9 23.8 9.9zm67.4-174.4L687.8 215l73.3 73.3-362.7 362.6-88.9 15.7 15.6-89zM880 836H144c-17.7 0-32 14.3-32 32v36c0 4.4 3.6 8 8 8h784c4.4 0 8-3.6 8-8v-36c0-17.7-14.3-32-32-32z"></path></svg></span> **Edit** — open the record for modification; and
- <span class="ams-ui-button ams-ui-button--small" aria-hidden="true"><svg viewBox="64 64 896 896" focusable="false"><path d="M360 184h-8c4.4 0 8-3.6 8-8v8h304v-8c0 4.4 3.6 8 8 8h-8v72h72v-80c0-35.3-28.7-64-64-64H352c-35.3 0-64 28.7-64 64v80h72v-72zm504 72H160c-17.7 0-32 14.3-32 32v32c0 4.4 3.6 8 8 8h60.4l24.7 523c1.6 34.1 29.8 61 63.9 61h454c34.2 0 62.3-26.8 63.9-61l24.7-523H888c4.4 0 8-3.6 8-8v-32c0-17.7-14.3-32-32-32zM731.3 840H292.7l-24.2-512h487l-24.2 512z"></path></svg></span> **Delete** — permanently remove a record when deletion is allowed.

Additional module-specific row actions may be available. Hover over an icon to see its label before selecting it.

Tables can also have actions below the rows. In most modules, a **New…** button opens a form for creating a record. Other tables may provide actions such as printing or starting a module-specific workflow.

!!! warning "Deleting records"
    Deletion can affect records linked elsewhere in AMS. Confirm that you selected the correct record and follow institutional policy before approving a deletion.

## Forms

Forms display and maintain one record. A form can open in three modes:

| Mode | Purpose |
|---|---|
| View | Review a record in read-only fields. |
| Create | Enter and submit a new record. |
| Edit | Change and submit an existing record. |

Required fields are marked in the form. Complete them and review every tab or section before selecting **Submit**. A successful submission creates or updates the record and normally returns you to its table.

Select **Close** to return to the module without submitting the current form. Existing records can also provide **Show Info**, which displays creation and update information and, where available, the audit log.

AMS includes several reusable controls whose behavior is more involved than a standard text field. See [Special form fields](special-form-fields.md) for selection fields with inline add/edit actions, dates, original-language metadata and translation, and repeatable field groups.
