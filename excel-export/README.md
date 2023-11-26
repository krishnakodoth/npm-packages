# Install

```javascript
npm i @krishnakodoth/excel-export
```

# Usage

```Javascript

import { ExcelExport } from "@krishnakodoth/excel-export";

const App = () => {
  const data=[
    {
      name: "Worksheet-1",
      border: false,
      data: {
        columns: [
          { header: "First Name", key: "firstName" },
          { header: "Last Name", key: "lastName" },
          { header: "Purchase Price", key: "purchasePrice" },
          { header: "Payments Made", key: "paymentsMade" },
        ],
        rows: [
          {
            firstName: "Kylie",
            lastName: "James",
            purchasePrice: 1000,
            paymentsMade: 900,
          },
          {
            firstName: "Harry",
            lastName: "Peake",
            purchasePrice: 1000,
            paymentsMade: 1000,
          },
        ],
      },
    },
    {
      name: "Worksheet-2",
      border: true,
      data: {
        columns: [
          { header: "First Name", key: "firstName" },
          { header: "Last Name", key: "lastName" },
          { header: "Purchase Price", key: "purchasePrice" },
          { header: "Payments Made", key: "paymentsMade" },
        ],
        rows: [
          {
            firstName: "Kylie",
            lastName: "James",
            purchasePrice: 1000,
            paymentsMade: 900,
          },
          {
            firstName: "Harry",
            lastName: "Peake",
            purchasePrice: 1000,
            paymentsMade: 1000,
          },
        ],
      },
    },
  ];
  return (
    <div>
      <ExportExcel
        excelData={data}
        buttonName={'button name'}
        className={'btn btn-primary'}
        fileName={'print_excel_file_name'}
      />
    </div>
  );
}

```
