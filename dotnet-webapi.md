# .NET WebApi
## Controller
### 檔案和類別命名
- 以**資源**來命名
- 使用開頭大寫
- 名詞複數
- 後置文字使用 `Controller`

範例
```csharp
StudentsController
CategoriesController
```

#### 如果遇到只使用單數資源，或名詞不可數，則使用單數命名

範例
```csharp
DataController
AccountController
```

### 欄位命名
- `private` 欄位應使用 `_` 作為前置文字
- 依照宣告的介面或類別來命名
- 盡量不使用縮寫
- `Service` 類的欄位使用 `s` 作為後置文字，當使用宣告資源類別複數的欄位時，前者須改用 `Service` 作為後置文字，表示複數的欄位應使用 `s` 作為後置文字

範例
```csharp
private ICustomerService _customers;
private Customer _customer;

private IManagerService _managerService;
private Manager[] _managers;
```

### Action 命名
- `Get`, `Find`, `FindAll`, `Create`, `Delete`, `Update`