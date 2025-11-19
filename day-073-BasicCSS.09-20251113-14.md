# Day 72 Part 2: Workshop - Design a Cafe Menu

Looking at the example project:
- there is a main, website-wide background image (the coffee beans)
- there is a block (if customize width instead of default full-width) or inline-block
- the block or inline-block has padding and margin, and a filled-in colour
- the content of the block container includes
  - bespoke font family and font size, weight
  - formatting like bold and italic
  - there are lines with red colour and top border
  - small icons/images under each category
  - rows of data `tr`, each row has two `td`: item name is left aligned, while price is right aligned
  - there is footer with hyperlink / anchor elements
  - there is footer with address bit

[Ends 21:09 13 Nov 2025]

[Starts 08:11 14 Nov 2025]

Wrote in VS Code the bones of the HTML and CSS (with a lot of placehodlers)\
```
<!DOCTYPE html>
<html>
    <head>
        <meta lang="UTF-8">
        <meta name="viewport" content="width=device-width initial-scale=1.0">
        <title>Build a Cafe Menu</title>
        <style>
            .box {
                width:
                height:
                background-color:
                margin:
            }
            #menu-header {
                font-family: ;
                font-size: ;
                font-weight: ;
            }
        </style>
        <!--something background image?-->
    </head>
    <body>
        <div class="box">
            <table id="menu-header">
                <thead>
                    <tr margin: ; padding: ;>
                        <td align="center" colspan="2"><b>CAMPER CAFE</b></td>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td align="center" colspan="2" margin: ; padding: ;><em>Est.2020</em></td>
                    </tr>
                    <tr>
                        <td colspan="2" border-line="" background-color="" margin: ; padding: ; width="" height=""></td>
                    </tr>
                </tbody>
            </table>
            <table id="menu-coffee">
                <thead>
                    <tr>
                        <td align="center" colspan="2" margin: ; padding: ;><b>Coffee</b></td>
                    </tr>
                    <tr>
                        <td margin: ; padding: ;><p><img src="" alt="steaming coffee in a cup" width="" height=""/></p></td>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td margin: ; padding: ;>French Vanilla</td>
                        <td align="right" margin: ; padding: ;>3.00</td>
                    </tr>
                    <tr>
                        <td margin: ; padding: ;>Caramel Macchiato</td>
                        <td align="right" margin: ; padding: ;>3.75</td>
                    </tr>
                    <tr>
                        <td margin: ; padding: ;>Pumpkin Spice</td>
                        <td align="right" margin: ; padding: ;>3.50</td>
                    </tr>
                    <tr>
                        <td margin: ; padding: ;>Hazelnut</td>
                        <td align="right" margin: ; padding: ;>4.00</td>
                    </tr>
                    <tr>
                        <td margin: ; padding: ;>Mocha</td>
                        <td align="right" margin: ; padding: ;>4.50</td>
                    </tr>
                </tbody>
            </table>
            <table id="menu-desserts">
                <thead>
                    <tr>
                        <td align="center" colspan="2" margin: ; padding: ;><b>Desserts</b></td>
                    </tr>
                    <tr>
                        <td margin: ; padding: ;><p><img src="" alt="a slice of cheesecake" width="" height=""/></p></td>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td margin: ; padding: ;>Donut</td>
                        <td align="right" margin: ; padding: ;>1.50</td>
                    </tr>
                    <tr>
                        <td margin: ; padding: ;>Cherry Pie</td>
                        <td align="right" margin: ; padding: ;>2.75</td>
                    </tr>
                    <tr>
                        <td margin: ; padding: ;>Chessecake</td>
                        <td align="right" margin: ; padding: ;>3.00</td>
                    </tr>
                    <tr>
                        <td margin: ; padding: ;>Cinnamon Roll</td>
                        <td align="right" margin: ; padding: ;>2.50</td>
                    </tr>
                    <tr>
                        <td colspan="2" border-line="black" background-color="red" margin: ; padding: ; width="" height=""></td>
                    </tr>
                </tbody>
            </table>
        </div>
    </body>
    <footer>
        <section id="wesbite">
            <p color="black" valign="center"><a href="https://www.freecodecamp.org">Visit our website</a></p>
        </section>
        <section>
            <address>
                <p>123 Free Code Camp Drive</p>
            </address>
        </section>
    </footer>
</html>
```
Renders o-kay-ish for a bone structure\
<img width="248" height="489" alt="image" src="https://github.com/user-attachments/assets/4bbac6cb-561c-42fd-969d-1419dac89061" />

[Ends 08:55 14 Nov 2025]


## What did go well
1. Not familiar with CSS as so far it's been only theory, but managed to get the table stuff at least I think 80% right
2. Still got the boilerplace in my mind after not been doing it for so long!
3. I now try to interprete the "page" from an HTML and CSS POV - good starting point despite the knowledge gap!

## What didn't go well

## Suggestions
