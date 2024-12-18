## testCreateProduct_Success()
ProductDTO productDTO = new ProductDTO();
productDTO.setName("Product C");
productDTO.setDescription("Description C");
productDTO.setColor("Green");
productDTO.setPrice(30.99);
productDTO.setStockQuantity(300);

assertNotNull(result.getId(), "Saved product should have an ID");
assertEquals("Product C", result.getName(), "Product name should match");
assertEquals("Description C", result.getDescription(), "Product description should match");
assertEquals("Green", result.getColor(), "Product color should match");
assertEquals(30.99, result.getPrice(), "Product price should match");
assertEquals(300, result.getStockQuantity(), "Product stock quantity should match");

## testCreateProduct_NegativePrice
ProductDTO productDTO = new ProductDTO();
productDTO.setName("Test Product");
productDTO.setDescription("Test Description");
productDTO.setColor("Blue");
productDTO.setPrice(-20.0); // invalid price!
productDTO.setStockQuantity(10);

## testGetAllProducts()
Product product1 = new Product();
product1.setId("1");
product1.setName("Product A");
product1.setDescription("Description A");
product1.setColor("Red");
product1.setPrice(10.99);
product1.setStockQuantity(100);

Product product2 = new Product();
product2.setId("2");
product2.setName("Product B");
product2.setDescription("Description B");
product2.setColor("Blue");
product2.setPrice(20.99);
product2.setStockQuantity(200);

assertNotNull(result, "The result should not be null");
assertEquals(2, result.size(), "There should be two products in the list");
assertEquals("Product A", result.get(0).getName(), "First product name should match");
assertEquals("Product B", result.get(1).getName(), "Second product name should match");

## testDeleteProduct_Success()
skriv själva!

## testDeleteProduct_NonExistentId()
skriv själva!
