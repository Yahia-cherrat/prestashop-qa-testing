# PrestaShop QA Testing

## Overview

This repository contains the QA testing deliverables for **Phase 2** of the PrestaShop Live Demo project.

The objective of this phase is to:

- Execute test cases and record the results
- Identify defects found during execution
- Document defects using bug reports
- Maintain traceability between test cases and defects
- Share the complete QA project through GitHub

## Application Under Test

**PrestaShop Live Demo – Front Office**

https://demo.prestashop.com/#/en/front

## Test Environment

- **Operating System:** Windows 11
- **Browser:** Google Chrome
- **Test Type:** Manual Testing
- **Application:** PrestaShop Live Demo

## Test Execution

The bidirectional matrix contains:

- Test Suite
- Test Case ID
- Test Title
- Test Type
- Preconditions
- Test Steps
- Expected Results
- Actual Results
- PASS / FAIL Status
- Defect Traceability

## Defects Identified

### BR-001 – Home page loads extremely slowly

**Related Test Case:** TC01  
**Type:** Non-functional / Performance  
**Status:** FAIL

The home page takes an unusually long time to load and become fully usable.

### BR-002 – Cart total is incorrect when two discounted products are added

**Related Test Case:** TC02  
**Type:** Functional / Pricing  
**Status:** FAIL

The displayed cart total can be at least `0.01` higher than the actual sum of the discounted product prices.

### BR-003 – Registered customer cannot sign in with valid credentials

**Related Test Case:** TC03  
**Type:** Functional / Authentication  
**Status:** FAIL

After creating an account and logging out, the customer cannot sign in again using the same valid credentials.

The application displays:

```text
Authentication failed.
