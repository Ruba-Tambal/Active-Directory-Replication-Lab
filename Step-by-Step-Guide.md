# Step-by-Step Guide - Active Directory Replication Lab

## 🎯 Objectives
- Deploy Primary and Additional Domain Controllers
- Configure DNS
- Verify replication
- Validate domain health

## STEP 1 — Create Resource Group & VMs
- Create `rg-ad-lab`
- Deploy `WIN2K25-DC01` (Primary DC)
- Deploy `WIN2K25-DC02` (Additional DC)

## STEP 2 — Configure DC01 (Primary Domain Controller)
1. Set static IP
2. Install AD DS role
3. Promote to Domain Controller
4. Configure DNS

## STEP 3 — Configure DC02 (Additional Domain Controller)
1. Join to domain
2. Install AD DS role
3. Promote as Additional DC

## STEP 4 — Verify Replication
tools -> Active Directory Sites and Services
```powershell
repadmin /replsummary
repadmin /showrepl
dcdiag /test:replications
