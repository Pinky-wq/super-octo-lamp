CREATE PROCEDURE usp_SearchProducts
    @ProductName NVARCHAR(255) = NULL,
    @Size INT = NULL,
    @Price DECIMAL(10, 2) = NULL,
    @MfgDate DATE = NULL,
    @Category NVARCHAR(50) = NULL
AS
BEGIN
    SELECT *
    FROM tbl_Product
    WHERE
        (ProductName = @ProductName OR @ProductName IS NULL)
        AND (Size = @Size OR @Size IS NULL)
        AND (Price = @Price OR @Price IS NULL)
        AND (MfgDate = @MfgDate OR @MfgDate IS NULL)
        AND (Category = @Category OR @Category IS NULL);
END;
