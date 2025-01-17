Document Management Settings
==============================

The following is available here, organized in three tabs:

General
*********
You can set this on the "General" tab:

.. image:: document-management-settings-general-new2.png

+ **Authors of Controlled Documents**: Here you can set the type of permissions to be used in Controlled Documents libraries in the tenant. 

    - "Document Authors Group": This is the default setting. A specific permission group will be used for authors.
    - "Site Owners": All site owners will have permissions to work with Controlled Documents. No specific permission group for authors is needed.
    - "Site Owners and Members": All site owners and all Members will have permissions to work with Controlled Documents. No specific permission group for authors is needed.
+ **Approvers Group**: If this option is selected (default) a specific permission group will be created for approvers in every Team Site with a Controlled Documents library. Note that this should normally be selected. Not using permission groups is for specialized implementation only. Also note that you can still set what type of approval to use for each Document Type.
+ **Archive Site Url**: Part of the Controlled Documents functionality is an Archive site, where a copy of all published document’s editions are placed in an archive. The link to the site is shown here and can be edited if needed.
+ **Retention Manager**: For retention of documents to work, a Retention Manager must be added in this field.

Document Id Format
*********************
Here you set the prefix for the Document id for this tenant.

.. image:: document-management-settings-format-new2.png

When a new controlled document is published the first time, a document id is set for the document, based on the prefix from the settings. This document id is then the same in all future editions of the document and is an important part of tracking published editions of the document. 

**Note!** The Document Format can be changed even after creation of Controlled Documents has started, but it's not really recommended. Still, if it's done, existing documents will keep their prefix and only new documents will get the new one.

Document Base Query
*********************
Here you can add one or more base queries that always should be executed in the background when a search is run in a rollup. The purpose is to help set what this organization regards as a "document". For example, is a PDF file regarded as a document?

Here's an example of a base query:

.. image:: document-management-base-query.png

You use Keyword Query Language (KQL) here. To learn more about KQL, see this Microsoft page: https://docs.microsoft.com/en-us/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference

