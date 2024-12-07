Al Khayat is a Moroccan traditional clothing company that manufactures and sell garments through a physical store, a website the promotes the sales of products in bulk and two retail e-commerece websites. 
The company uses Odoo for their website needs and inventory management and is try to cartography its IT infrastructure and rationalize its process for more sales, less wasted raw materials, better quality.

- Overview of the **Current** supply/production chain: 
	- Raw materials (Fabric/Yarn) are delivered to a warehouse
	- Yarn is transformed to clothing components used to decorate the garments
	- Fabric is cut and transformed into pieces (front/back/pockets...).
	- The **Cut Fabric and its Yarn based pieces are bundled** and chipped to a processing facility.
	- The processing facility assembles the bundled items creating the garments and ships them back.
	- Each product goes through a **Quality Assessment** step where the product is checked for (true size, holes, missing components...),
		- If the product fails QA its either sent back to the processing facility or sent to be a laundry service on premise.

- Overview of areas of where the Odoo ERP could intervene to make the chain better 
	 - Add **Internal Reference** on the bundled pieces before shipping to processing facility to facilitate the **QA** process.
		 - *Option 1*: During the cutting of the cloth pre-prepared stickers with the Internal reference of the product are stuck on each piece.
			 - *Questions*: 
				 - Does the internal reference make reference to the products attributes ? (color, size,....) 
				 - Does the cutting process done for each product by their attribute ? (to allow for time to change/prepare the stickers for the next batch) 
		 - *Option 2*: During the bundling of the fabric pieces and their components a sticker with the internal reference is attached.

*References:* To help keep track of product from within a warehouse and its routes we cause:
	https://www.odoo.com/documentation/17.0/applications/inventory_and_mrp/inventory/warehouses_storage/inventory_management/use_routes.html#use-routes-and-rules