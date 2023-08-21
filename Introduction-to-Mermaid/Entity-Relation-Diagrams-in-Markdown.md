
::: mermaid
erDiagram
      CUSTOMER }|--|{ DELIVERY-ADDRESS : has
      CUSTOMER ||--o{ ORDER : places 
      CUSTOMER ||..o{ INVOICE : "    "
      INVOICE ||--|{ ORDER : covers
      DELIVERY-ADDRESS ||..o{ ORDER : receives
      ORDER ||--|{ ORDER-ITEM : includes
      PRODUCT-CATEGORY ||..|{ PRODUCT : contains
      PRODUCT ||--o{ ORDER-ITEM : "ordered in"
:::
