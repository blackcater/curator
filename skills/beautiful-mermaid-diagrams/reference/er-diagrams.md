# ER Diagram Examples

## Basic relationship

```mermaid
erDiagram
  CUSTOMER ||--o{ ORDER : places
```

## Entity with attributes

```mermaid
erDiagram
  CUSTOMER {
    int id PK
    string name
    string email UK
    date created_at
  }
```

## Attribute keys (PK, FK, UK)

```mermaid
erDiagram
  ORDER {
    int id PK
    int customer_id FK
    string invoice_number UK
    decimal total
    date order_date
    string status
  }
```

## Exactly One to Exactly One

```mermaid
erDiagram
  PERSON ||--|| PASSPORT : has
```

## Exactly One to Zero-or-Many

```mermaid
erDiagram
  CUSTOMER ||--o{ ORDER : places
```

## Zero-or-One to One-or-Many

```mermaid
erDiagram
  SUPERVISOR |o--|{ EMPLOYEE : manages
```

## One-or-More to Zero-or-Many

```mermaid
erDiagram
  TEACHER }|--o{ COURSE : teaches
```

## All cardinality types

```mermaid
erDiagram
  A ||--|| B : OneToOne
  C ||--o{ D : OneToMany
  E |o--|{ F : OptToMany
  G }|--o{ H : ManyToMany
```

## Identifying relationship

```mermaid
erDiagram
  ORDER ||--|{ LINE_ITEM : contains
```

## Non-identifying relationship

```mermaid
erDiagram
  USER ||..o{ LOG_ENTRY : generates
  USER ||..o{ SESSION : opens
```

## Mixed identifying & non-identifying

```mermaid
erDiagram
  ORDER ||--|{ LINE_ITEM : contains
  ORDER ||..o{ SHIPMENT : ships-via
  PRODUCT ||--o{ LINE_ITEM : includes
  PRODUCT ||..o{ REVIEW : receives
```

## E-commerce schema

```mermaid
erDiagram
  CUSTOMER {
    int id PK
    string name
    string email UK
  }
  ORDER {
    int id PK
    date created
    int customer_id FK
  }
  PRODUCT {
    int id PK
    string name
    float price
  }
  LINE_ITEM {
    int id PK
    int order_id FK
    int product_id FK
    int quantity
  }
  CUSTOMER ||--o{ ORDER : places
  ORDER ||--|{ LINE_ITEM : contains
  PRODUCT ||--o{ LINE_ITEM : includes
```

## Blog platform schema

```mermaid
erDiagram
  USER {
    int id PK
    string username UK
    string email UK
    date joined
  }
  POST {
    int id PK
    string title
    text content
    int author_id FK
    date published
  }
  COMMENT {
    int id PK
    text body
    int post_id FK
    int user_id FK
    date created
  }
  TAG {
    int id PK
    string name UK
  }
  USER ||--o{ POST : writes
  USER ||--o{ COMMENT : authors
  POST ||--o{ COMMENT : has
  POST }|--o{ TAG : tagged-with
```

## School management schema

```mermaid
erDiagram
  STUDENT {
    int id PK
    string name
    date dob
    string grade
  }
  TEACHER {
    int id PK
    string name
    string department
  }
  COURSE {
    int id PK
    string title
    int teacher_id FK
    int credits
  }
  ENROLLMENT {
    int id PK
    int student_id FK
    int course_id FK
    string semester
    float grade
  }
  TEACHER ||--o{ COURSE : teaches
  STUDENT ||--o{ ENROLLMENT : enrolled
  COURSE ||--o{ ENROLLMENT : has
```
