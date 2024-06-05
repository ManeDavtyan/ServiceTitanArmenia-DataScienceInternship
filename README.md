# ServiceTitanArmenia-DataScienceInternship
The provided script `DataExtraction.ipynb` creates a DataExtractor class that has the functionality to load the dataset and transform the unstructured data into a flat data with the following columns:
-invoice_id: int
-created_on: datetime64[ns]
-invoiceitem_id: int
-invoiceitem_name: str
-type: str (use this conversion table: {0: 'Material', 1: 'Equipment', 2: 'Service', 3: 'Other'})
-unit_price: int
-total_price: int (unit_price*quantity)
-percentage_in_invoice: float (unit_price*quantity / invoice_total)
-is_expired: bool (whether invoice_id is contained expired_invoices.txt or not)



The resulting .csv file is stored as `results.csv`.
