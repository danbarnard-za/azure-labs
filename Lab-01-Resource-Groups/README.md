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

```text
Subscription
│
├── RG-IT-Prod
│     └── Storage Account
│
└── RG-IT-Test
```

---

## Lab Steps

### Step 1 – Create Resource Group

Created a Resource Group named **RG-IT-Prod** in the South Africa North region.

![RG Created](Lab-01-Resource-Groups/images/01-resource-group-created.png)

---

### Step 2 – Create Storage Account

Created a Standard Storage Account inside **RG-IT-Prod**.

![Storage Account](images/02-storage-account.png)

---

### Step 3 – Apply Tags

Applied the following tags:

| Tag | Value |
|-----|-------|
| Environment | Production |
| Department | IT |
| Owner | Dan |

![Tags](images/03-tags.png)

---

### Step 4 – Move Resource

Moved the Storage Account from **RG-IT-Prod** to **RG-IT-Test**.

![Move](images/04-move-resource.png)

---

### Step 5 – Delete Resource Groups

Deleted **RG-IT-Prod**.

Attempted to delete **RG-IT-Test**.

Azure initially prevented deletion because the Storage Account had a pending geo-redundancy change.

---


## Screenshots

_To be added._

## Lessons Learned

Issue - Resource Group deletion failed with ResourceGroupDeletionBlocked and PendingTransactionAlreadyExists.
Cause - The Storage Account redundancy had just been changed from RA-GRS to LRS, triggering a backend geo-replication update. Azure blocked deletion until that operation completed.
Resolution - Waited for the Storage Account provisioning/replication update to finish, then retried the Resource Group deletion successfully.
Observation: Attempting to delete a Resource Group can fail if one of its resources has a pending management operation (such as changing Storage Account redundancy). Azure rolls back the Resource Group deletion until the operation completes.


## Troubleshooting

_To be added._
