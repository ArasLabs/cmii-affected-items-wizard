# CMII Affected Items Wizard

Interactive Wizard that helps analyze which Items (Parts or Documents) should be added to the ECR Affected Items Tab.

It implements rules that guides the user to consider additional Documents and Parts that should be evaluated. The wizard records decisions made about impact (or not) and records for traceability, who made the decisions.

## History

This project and the following release notes have been migrated from the old Aras Projects page.

Release | Notes
--------|--------
[v9](https://github.com/ArasLabs/cmii-affected-items-wizard/releases/tag/v9) | 9.13.2011 Updated for compatibility with 9.3 (v8.2 should be used for Aras Innovator versions prior to 9.3)
[v8.2](https://github.com/ArasLabs/cmii-affected-items-wizard/releases/tag/v8.2) | 09.21.2010 Updated merge additional changes
[v8.1](https://github.com/ArasLabs/cmii-affected-items-wizard/releases/tag/v8.1) | 02.04.2010 Updated to remove Default Life Cycle from ECR Affected Wizard Item ItemType.
[v8](https://github.com/ArasLabs/cmii-affected-items-wizard/releases/tag/v8) | 04.08.2009 Updated for Version 9.1, and integrated to the new Simple ECO itemType
[v7](https://github.com/ArasLabs/cmii-affected-items-wizard/releases/tag/v7) | 01.21.2009 (peter) updated and tested on v9.0.2 of Innovator. 3 package changes: (1) Removed the error message about missing ItemType when there are un-saved Affected items when the Wizard is opened (2) List of change controlled itemtypes is now dynamic. For example, if a new itemType named Tool is created with a Relationship "Part Tool" then the wizard will adapt to this new itemType. This removes the hardcoding of Part and Document as the only controlled items. (3) CMII Wizard is now also connected to the ECN.
[v6](https://github.com/ArasLabs/cmii-affected-items-wizard/releases/tag/v6) | 06/27/2008 (Peter) updated the package for Innovator 8.2.0 and 9.0.1 Also made the Lookup function work with filtered values. WARNING: ACTUNG: I have changed the name of the package to just CMIIAffectedItemsWizard, dropping the "com.aras.innovator.solution." prefix. You must rename the Package you already have loaded in Innovator, before you can merge the new versions changes in.
[v4](https://github.com/ArasLabs/cmii-affected-items-wizard/releases/tag/v4) | 09/27/2007 (Peter) this release was packaged after the CMII Conference in Washington. Now supports version 8.1.1 and has improved error handling. The entre solution is now a package (no external files).
[v1](https://github.com/ArasLabs/cmii-affected-items-wizard/releases/tag/v1) | Initial Release - the result of the RobMcAveney, Peter Schroer and Mike Gavlak collaboration

#### Supported Aras Versions

Project | Aras
--------|------
[v9](https://github.com/ArasLabs/cmii-affected-items-wizard/releases/tag/v9) | 9.3
[v8.2](https://github.com/ArasLabs/cmii-affected-items-wizard/releases/tag/v8.2) | 9.1
[v8.1](https://github.com/ArasLabs/cmii-affected-items-wizard/releases/tag/v8.1) | 9.1
[v8](https://github.com/ArasLabs/cmii-affected-items-wizard/releases/tag/v8) | 9.1
[v7](https://github.com/ArasLabs/cmii-affected-items-wizard/releases/tag/v7) | 9.0.2
[v6](https://github.com/ArasLabs/cmii-affected-items-wizard/releases/tag/v6) | 8.2.0, 9.0.1
[v4](https://github.com/ArasLabs/cmii-affected-items-wizard/releases/tag/v4) | 8.1.1
[v1](https://github.com/ArasLabs/cmii-affected-items-wizard/releases/tag/v1) | 8.0.0

## Installation

#### Important!
**Always back up your code tree and database before applying an import package or code tree patch!**

### Pre-requisites

1. Aras Innovator installed
2. Aras Package Import tool
3. **CMIIAffectedItemsWizard** import package

> *Note: The Package name has been changed with v6.*
> 
> This will only impact you if you already have a previous version loaded. Before you can successfully import this new version, you must either rename the package (Administration-->Packages) to CMIIAffectedItemsWizard (removing the com.aras),  or Delete the Package item.

### Install Steps

1. Backup your database and store the BAK file in a safe place.
2. Open up the Aras Package Import tool.
3. Enter your login credentials and click **Login**
    * _Note: You must login as root for the package import to succeed!_
4. Enter the package name in the TargetRelease field.
    * Optional: Enter a description in the Description field.
5. Enter the path to your local `..\CMIIAffectedItemsWizard\Import\imports.mf` file in the Manifest File field.
6. Select all in the Available for Import field.
7. Select Type = **Merge** and Mode = **Thorough Mode**.
8. Click **Import** in the top left corner.
9. Close the Aras Package Import tool.

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request

## Credits

Created by Rob McAveney, Peter Schroer, and Mike Gavlak at Aras Corporation.

## License

Published to Github under the MIT license. See the [LICENSE file](./LICENSE.md) for license rights and limitations.
