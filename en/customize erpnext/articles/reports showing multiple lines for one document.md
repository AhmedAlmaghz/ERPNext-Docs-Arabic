**Question:**

I have made a report on Purchase Invoice. Why following Invoice is being shown twice in the report?

![](https://docs.erpnext.com/files/3w1roiE.png)

**Answer:**

It must be because in the Pick Columns, you have selected a field from Child Table (like Item or taxes table). Since that table has two rows, it's been shown twice in the report. Just scroll to far-right to confirm.

![](https://docs.erpnext.com/files/BFinlvC.png)