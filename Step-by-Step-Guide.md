# Step-by-Step Guide - Active Directory Replication Lab

## 🎯 Objectives
- Deploy Primary and Additional Domain Controllers
- Configure DNS integrated with Active Directory
- Verify replication between DCs
- Validate domain health using diagnostic tools

## STEP 1 — Create Resource Group & VMs
- Create Resource Group: `rg-ad-lab`
- Deploy `WIN2K25-DC01` (Primary Domain Controller)
- Deploy `WIN2K25-DC02` (Additional Domain Controller)

## STEP 2 — Configure DC01 (Primary Domain Controller)
1. Set static IP address
2. Install AD DS role
3. Promote server to Domain Controller
4. Configure DNS

## STEP 3 — Configure DC02 (Additional Domain Controller)
1. Join DC02 to the domain
2. Install AD DS role
3. Promote as Additional Domain Controller

## STEP 4 — Verify Replication
Run the following commands on DC01 or DC02:

```powershell
# 1. Replication Summary
repadmin /replsummary

# 2. Detailed Replication Status
repadmin /showrepl

# 3. Domain Health Check
dcdiag /s:WIN2K25-DC01

# 4. Test Replication Specifically
dcdiag /test:replications
STEP 5 — Validation

Open Active Directory Users and Computers
Open DNS Manager
Open Active Directory Sites and Services and check replication status

Lab Completed Successfully! 🎉
text---

### **How to update it on GitHub:**

1. Go to your repository.
2. Open the file `Step-by-Step-Guide.md`
3. Click the **pencil icon** (Edit)
4. Delete the old content and paste the new one above.
5. Scroll down and click **Commit changes**.

This will make Step 5 and the commands look clean and professional.

---

Would you like me to update the full set of files (`README.md`, `Verification.md`, etc.) with this style?how make step 5 dont effect by command style✅ Here is the updated Step-by-Step-Guide.md with Step 5 formatted as normal text (no command block style):

Markdown# Step-by-Step Guide - Active Directory Replication Lab

## 🎯 Objectives
- Deploy Primary and Additional Domain Controllers
- Configure DNS integrated with Active Directory
- Verify replication between DCs
- Validate domain health using diagnostic tools

## STEP 1 — Create Resource Group & VMs
- Create Resource Group: `rg-ad-lab`
- Deploy `WIN2K25-DC01` (Primary Domain Controller)
- Deploy `WIN2K25-DC02` (Additional Domain Controller)

## STEP 2 — Configure DC01 (Primary Domain Controller)
1. Set static IP address
2. Install AD DS role
3. Promote server to Domain Controller
4. Configure DNS

## STEP 3 — Configure DC02 (Additional Domain Controller)
1. Join DC02 to the domain
2. Install AD DS role
3. Promote as Additional Domain Controller

## STEP 4 — Verify Replication
Run the following commands on DC01 or DC02:

```powershell
# Replication Summary
repadmin /replsummary

# Detailed Replication Status
repadmin /showrepl

# Domain Health Check
dcdiag /s:WIN2K25-DC01

# Test Replication Specifically
dcdiag /test:replications

STEP 5 — Validation

Open Active Directory Users and Computers
Open DNS Manager
Open Active Directory Sites and Services and check replication status between the two Domain Controllers

Lab Completed Successfully! 🎉
