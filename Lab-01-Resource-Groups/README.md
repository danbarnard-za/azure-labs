# Lab 01 – Resource Groups

## Objective

Learn how to create, manage and organize Azure resources using Resource Groups.

## Technologies

- Azure Resource Groups
- Azure Storage Account
- Azure Tags

## Lab Tasks

- [x] Create a Resource Group
- [x] Create a Storage Account
- [x] Apply Tags
- [x] Move the Storage Account to another Resource Group
- [x] Delete the Resource Groups

## Architecture

_To be added._

## Screenshots

_To be added._

## Lessons Learned

Issue - Resource Group deletion failed with ResourceGroupDeletionBlocked and PendingTransactionAlreadyExists.
Cause - The Storage Account redundancy had just been changed from RA-GRS to LRS, triggering a backend geo-replication update. Azure blocked deletion until that operation completed.
Resolution - Waited for the Storage Account provisioning/replication update to finish, then retried the Resource Group deletion successfully.
Observation: Attempting to delete a Resource Group can fail if one of its resources has a pending management operation (such as changing Storage Account redundancy). Azure rolls back the Resource Group deletion until the operation completes.


## Troubleshooting

_To be added._
