# TKCSDL_20212
/*
-- non-index
SELECT * FROM HumanResources.Employee AS DATA
WHERE LOWER(DATA.JobTitle) LIKE '%design%'
*/

/*
--index
SELECT * FROM HumanResources.Employee_Index AS DATA
WHERE LOWER(DATA.JobTitle) LIKE '%design%'
*/

/*
--clustered index
SELECT * INTO HumanResources.Employee_Clustered_Index FROM HumanResources.Employee
USE AdventureWorks2019
GO
SELECT * FROM HumanResources.Employee_Clustered_Index AS DATA
WHERE LOWER(DATA.JobTitle) LIKE '%design%'
*/

/*
--non-clustered-index
SELECT * INTO HumanResources.Employee_NonClustered_Index FROM HumanResources.Employee
USE AdventureWorks2019
GO
SELECT * FROM HumanResources.Employee_NonClustered_Index AS DATA
WHERE LOWER(DATA.JobTitle) LIKE '%design%'
*/
