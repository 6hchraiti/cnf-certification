## How to review CNF Certification results

### Technical Requirements

1. Verify that the list of files matches the [expected list](https://github.com/cncf/cnf-certification/blob/main/instructions.md#contents-of-the-pr).
1. Note the vX.Y subdirectory that the PR is in, this is the version of CNF Certification for which certified is being claimed, referenced as the "Certification Version" from hereon.
1. Verify that the Certification Version is the current or previous version of CNF Certification.
1. Look at results log, cnf-testsuite-results-YYYY-MMDD-HHMMSS-NNN.yml. Verify that the major.minor component of the CNF Certification match the certification version being claimed. The patch version does not matter.
1. Verify that the RESULTS SUMMARY section of results log "X of Y essential tests passed". There should be at least 10 essential tests passed.

### Policy Requirements
1. Confirm that the vendor is currently a member of CNCF. If they are not, request that they reach out to memberships@cncf.io to become a member in order to complete their certification. (Companies can alternatively pay a certification fee equal to the cost of membership if, for whatever reason, they don't wish to become a CNCF member.) Alternatively, non-profit organizations (including community distributions like Debian) can certify at no cost.

Review the PRODUCT.yaml file, and:

2. Verify that there is a Participation Form on file for the vendor, and that the vendor is in good standing in the program.
3. Verify the product name, product version and website_url are listed in the "Qualifying Offerings" section of the vendor's Participation Form.

If the submission doesn't meet all policy requirements, reply with a message indicating "Signed participation form needed", "Files missing from PR", "Membership in CNCF or confirmation of non-profit status needed", etc.

### Tasks to Complete After Review
1. Update the Certified CNF spreadsheet to reflect the vendor's certified offering.
2. Add the vendor's information to the CNCF landscape which also causes them to appear on https://www.cncf.io/certification/cnf.
3. Add a comment saying "This product is now a "Certified CNF".
4. Merge the PR (eg. Squad and merge).
5. Close the PR.
