# A framework for managing IT operations in a business

This framework is a condensation of my experience in IT Support, IT Systems and Network Administration (and IT Management) of over a decade.

The goal is to simplify and streamline the organisation of information in the most intuitive and easily maintainable way.

Up till now, I have stored it in OneNote format and I began the process of converting it to markdown and other filetypes in this github repository in May 2022.

## Future plans

I have plans to build an app which will realise this framework in a convenient and powerful format to bring Enterprise grade IT management practices into the reach of small, solo or even part time IT professionals.

For now, I'm offering the framework in text format which may still hopefully improve somebody's life.

# Areas

We have different types of things we need to keep.

- physical files (licensing files, visio diagrams, pdfs, etc)
- notes and information (knowlegebase articules, procedures, checklists and records of activity)

Until now, I've had two separate areas. Physical files were stored in a windows folder structure. In most jobs this was a network shared folder, most recently it is a Teams based sharepoint folder (in practice, the same since OneDrive can mount it in explorer and it becomes just another folder).

Now that I have learnt to use git and become more familiar with markdown, and considering moving the knowledgebase type information from OneNote into Markdown files, I'm considering combining the two into one single project. This of course would only be suitable if all those accessing the information and files are comfortable with git and git repositories like Gitlab, and Github.

Often, as IT professionals we need to make documentation available to people who aren't comfortable with different tools (usually management), or live under restrictions (usually helpdesk). In these cases it might be the best choice to continue maintaining files and information in a windows share.

### Physical Files

For the first, I propose a folder structure which classifies everything into logical compartments.
This is stored in an ITAdmin share or Teams sharepoint folder or somewhere similar.

See [folder-structure.md](./physical-folder-structure.md)

### Notes and knowledge

I propose to store these as markdown files at the moment.
See [folder-structure.md](./documentation-structure.md)

<pre>
<code>
root/
├─ Policies and Registers/
│  ├─ Registers/
│  │  ├─ <a href="https://github.com/gostega/itops-framework/blob/main/Documentation%20Structure/Registers/Register%20of%20Documents.md">Register of Documents.md</a>
│  │  ├─ Register of Shares and Folders.md</a>
│  │  ├─ Register of Known Security Issues.md</a>
│  │  ├─ Register of Physical Media.md</a>
│  │  ├─ Register of Credit Card Usage.md</a>
│  │  └─ Register of Business Information.md</a>
│  ├─ Policies/
│  │  ├─ Terms and Definitions.md</a>
│  │  ├─ Asset Policies and Principles.md</a>
│  │  ├─ Archive and Backup Disk Policy.md</a>
│  │  ├─ Data Protection and Privacy.md</a>
│  │  ├─ Data Retention Lifecycle.md</a>
│  │  ├─ Corporate Account Security.md</a>
│  │  ├─ Staff Password Policy.md</a>
│  │  └─ AWS Resource Policy.md</a>
│  ├─ Specifications and Reference Tables/
│  │  ├─ Asset Labelling Conventions.md</a>
│  │  ├─ Naming Conventions.md</a>
│  │  ├─ Service Importance Levels.md</a>
│  │  ├─ Network Patch Lead Specs.md</a>
│  │  └─ IT Worklog Breakdown</a>
├─ Appliances/
│  ├─ Appliance Template.md
│  ├─ Dell Equalogic.md
│  └─ UPS - APC.md
├─ Apps/
│  ├─ aduc.tf
│  └─ dns.tf
├─ Configuration Items/
├─ Change/
├─ Fixes/
├─ Goals & Strategy/
├─ Procedures/
├─ Resources/
├─ Security/
├─ Services/
├─ Software/
├─ User Management/
└─ README.md
</code>
</pre>
