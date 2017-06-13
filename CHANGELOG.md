## V8 of the CMII Affected Items Wizard

Changes:

- Added Link to the new ECO itemType

- Tested for v9.1

## V7 of the CMII Affected Items Wizard

Changes:

- Removed the error message about missing ItemType when there are un-saved Affected items when the Wizard is opened

- List of change controlled itemtypes is now dynamic.  
    - For example, if a new itemType named Tool is created with a Relationship "Part Tool" then the wizard will adapt to this new itemType. This removes the hardcoding of Part and Document as the only controlled items.

- Tested for v9.0.2

## V6 of the CMII Affected Items Wizard

- The Package name was changed with v6. This will only impact you if you already have a previous version (earlier than 6) already loaded. 

- Before you can successfully import this new version, you must either rename the package (Administration-->Packages) to CMIIAffectedItemsWizard (removing the com.aras), or Delete the Package item.
