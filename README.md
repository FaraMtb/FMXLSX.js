# FMXLSX.js
Export JSON to ToExcel CSV/XLS/XLSX/Txt 
FMXLSX is a jQuery dependent JavaScript library to download or create Excel CSV/XLS/XLSX/Text spreadsheets using JavaScript (JSON).

This library is fully dynamic and flexible we can merge and set styling on each cell. Useful for creating an online JSON/JS Objects To (CSV/XLS/XLSX/Text spreadsheet) converter.

The plugin uses jQuery ,js-xlsx: Spreadsheet parser and writer
FileSaver.js: HTML5 saveAs() FileSaver implementation

installation:

<script src=".../plugins/FMXLSX/FMXLSX.js'" ></script> 


                    var data = [
                      { "Name": "Otto Clay", "Age": 25, "Country": 1, "Address": "Ap #897-1459 Quam Avenue", "Married": false },
                      { "Name": "Connor Johnston", "Age": 45, "Country": 2, "Address": "Ap #370-4647 Dis Av.", "Married": true },
                      { "Name": "Lacey Hess", "Age": 29, "Country": 3, "Address": "Ap #365-8835 Integer St.", "Married": false },
                      { "Name": "Timothy Henson", "Age": 12, "Country": 1, "Address": "911-5143 Luctus Ave", "Married": true },
                      { "Name": "Otto Clay", "Age": 1, "Country": 1, "Address": "Ap #897-1459 Quam Avenue", "Married": false },
                      { "Name": "Connor Johnston", "Age": 45, "Country": 2, "Address": "Ap #370-4647 Dis Av.", "Married": true },
                      { "Name": "Lacey Hess", "Age": 29, "Country": 3, "Address": "Ap #365-8835 Integer St.", "Married": false }];
                      var fileOptions = [
                          {
                              "sheetName": "Sheetname",
                             
                          }
                      ];
                      function save() {
                          var options = {
                              fileName: "Export Sheet",
                              fileType: "xlsx",
                              extension: ".xlsx",
                          };
                      fileColumns=[{ "Name": "Name", "Age": "Age", "Country": "Country", "Address": "Address", "Married": "Married" }
                            ];
                          fmxlsx.export(fileOptions,fileColumns,data ,options);
                      }
                      save();
