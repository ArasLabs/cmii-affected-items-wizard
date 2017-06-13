# CMII Affected Items Wizard

Interactive Wizard that helps analyze which Items (Parts or Documents) should be added to the ECR Affected Items Tab.

It implements rules that guides the user to consider additional Documents and Parts that should be evaluated. The wizard records decisions made about impact (or not) and records for traceability, who made the decisions.

## History

This project and the following release notes have been migrated from the old Aras Projects page.

Release | Notes
--------|--------
[v1](https://github.com/ArasLabs/cmii-affected-items-wizard/releases/tag/v1) | Initial Release - the result of the RobMcAveney, Peter Schroer and Mike Gavlak collaboration

#### Supported Aras Versions

Project | Aras
--------|------
[v1](https://github.com/ArasLabs/cmii-affected-items-wizard/releases/tag/v1) | 8.0.0

## Installation

#### Important!
**Always back up your code tree and database before applying an import package or code tree patch!**

### Pre-requisites

1. Aras Innovator installed
2. Aras Package Import tool
3. **CMIIAffectedItemsWizard** import package
4. **CMIIAffectedItemsWizard** code tree patch

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
10. Backup your code tree (the Aras install directory) and save the backup in a safe place.
11. Copy the `Innovator/` folder from the `CodeTree/` directory and paste it into the root directory of your Aras installation. 
12. Clear your browser cache before logging in to Aras.

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
