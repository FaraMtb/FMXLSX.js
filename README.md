# FMXLSX.js
Export JSON to ToExcel CSV/XLS/XLSX/Txt 
FMXLSX is a jQuery dependent JavaScript library to download or create Excel CSV/XLS/XLSX/Text spreadsheets using JavaScript (JSON).

This library is fully dynamic and flexible we can merge and set styling on each cell. Useful for creating an online JSON/JS Objects To (CSV/XLS/XLSX/Text spreadsheet) converter.


var fileOptions = [
                          {
                              "sheetName": "Sheetname",
                             
                          }
                      ];
                      function save() {
                          var options = {
                              fileName: "Export Sheet",
                              fileType: "csv",
                              extension: ".csv",
                          };
                      fileColumns=[{ "Name": "Name", "Age": "Age", "Country": "Country", "Address": "Address", "Married": "Married" }
                            ];
                          Jhxlsx.export(fileOptions,fileColumns,data ,options);
                      }
                      save();
