# markdowndemo.github.io
# Hello World
## 你好
### 形势大好
1. First item
2. Second item
3. Third item
- First item
- Second item
- Third item
[markdownguide](https://www.markdownguide.org/cheat-sheet/)

```
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
```
- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media

~~The world is flat.~~
	term
: definition

### My Great Heading {#custom-id}

Here's a sentence with a footnote. [^1]

[^1]: This is the footnote.

| Syntax | Description |
| ----------- | ----------- |
| Header | Title |
| Paragraph | Text |

I just love **bold text**.
I just love __bold text__.
Love**is**bold


Italicized text is the *cat's meow*.	

This text is ***really important***.	

> #### The quarterly results look great!
>
> - Revenue was off the chart.
> - Profits were higher than ever.
>
>  *Everything* is going according to **plan**.

- First item
- Second item
- Third item
    - Indented item
    - Indented item
    	- HEllo
- Fourth item

<https://www.markdownguide.org>
<fake@example.com>

const ExcelJS = require('exceljs');
const fs = require('fs')

```javascript
async function a() {
    const workbook = new ExcelJS.Workbook();
    const filename = 'D:\\Amomun\\DQE.xlsx';
    console.log(filename);
    await workbook.xlsx.readFile(filename)
        .then(function () {
            console.log('Hello World')
            let worksheet = workbook.getWorksheet('My Sheet');
            var imageId2 = workbook.addImage({
                filename: 'tek00000.png',
                extension: 'png',
              });
            worksheet.addImage(imageId2, 'B2:D6');
            /*worksheet.mergeCells('A1:B2');
            worksheet.getCell('A1').value = 'I am merged';
            worksheet.getCell('C1').value = 'I am not';
            worksheet.getCell('C2').value = 'Neither am I';*/
            //worksheet.getRow(2).commit(); 
            console.log('Finish')
        })
    await workbook.xlsx.writeFile(filename)
    //await workbook.commit();
}
a();
```
