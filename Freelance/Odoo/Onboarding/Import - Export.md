## Create Product Categories:

## Import Product Attributes:
Then Export them while making sure we export the external ID we will need to upload the Product Template (Parent Product).
*note: You can find a pre-defined export template of Attribute (insert screenshot)*

## Import Product Templates (Parent Products):
- **Step 1: Export Products Attributes with their External IDs**
use the attributes_for_parent_products template
![[attributes_for_parent_products_1.gif]]
- **Step 2: Fill out the Parent Product Template**
use the parent_product_template template to export and example then add the products you want to create with their attribute external id and its values external id(s)
![[parent_product_template.gif]]
## Set Variants Internal Reference:
To do this we need to head to the Products->Products Variants page and export the automatically created variants using the *pre-defined export template* 
![[Pasted image 20231212121258.png]]
Then for each Variant we can set the Internal Reference as well as other information (barcode, description.....).
![[internal_refrence_template.gif]]
## Set Stock 
1st step is to export the product variants and export the inventory adjustment template and fill it
**Step 1: Export Products variants**
Export the variants with their External IDs. Choose the export_variants_with_external_id template when exporting.
![[export_variants_with_external_id_2 1.gif]]
**Step 2: Fill out the Inventory Adjustments Import file**
- Start by exporting an example using the pre-made template (init_inventory_template)
![[filling_out_Inventory_Adjustments_1.gif]]
- Then add the new Variant stock count and make sure to add the *product_id/id* (The Variant External ID we exported in step 1). Also make sure to create and a unique id for the newly created Inventory Adjustment record we will create. 
	The GIF bellow showcases this step in detail. 
	*Note:
	 - The spreadsheet on the left is the Inventory Adjustments Template we will upload and the spreadsheet on the rihgt is the Products Variants with External ID (product_id/id) we need to fill Inventory Adjustments Template*.
	 - In the GIF we delete the 1st record because we can only import stock for new products that do not already exist in the Inventory Adjustments list.
![[filling_out_Inventory_Adjustments_2.gif]]

![[filling_out_Inventory_Adjustments_2 1.gif]]

**Step 3: Updating the stock**
To set the stock of variants we need to head to the Operations->Physical Inventory Page and click on **Apply All** then we need attribute a **Counted Quantity Value** for each of the product variants.

![[set_stock.gif]]