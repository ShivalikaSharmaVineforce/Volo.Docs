# Parameters

This document defines the configurable parameters for the **AssetManagementDocs** project, which manages assets across various locations, tracks statuses, and assigns responsibilities.

## Parameter 1: `assetId`
- **Description:** Unique identifier for each asset in the system.
- **Type:** `String`
- **Required:** ✅ Yes
- **Example:** `ASSET-000145`

## Parameter 2: `locationCode`
- **Description:** Represents the location or branch where the asset is stored or deployed.
- **Type:** `String`
- **Required:** ❌ No
- **Example:** `LOC-NY-003`

## Parameter 3: `status`
- **Description:** Current lifecycle status of the asset.
- **Accepted Values:** `Active`, `Inactive`, `Maintenance`, `Disposed`
- **Type:** `String`
- **Required:** ❌ No
- **Example:** `Active`

## Parameter 4: `assignedTo`
- **Description:** User or employee to whom the asset is currently assigned.
- **Type:** `String`
- **Required:** ❌ No
- **Example:** `john.doe`

## Parameter 5: `category`
- **Description:** Type/category of the asset such as vehicle, equipment, or IT hardware.
- **Type:** `String`
- **Required:** ❌ No
- **Example:** `IT-Equipment`

---

## Example Usage

Here's an example of how these parameters might be passed to a CLI tool or API:

```bash
asset-cli assign \
  --assetId ASSET-000145 \
  --locationCode LOC-NY-003 \
  --status Active \
  --assignedTo john.doe \
  --category IT-Equipment
