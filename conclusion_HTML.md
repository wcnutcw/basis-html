
utf-8 : ภาษาไทย
<head>...</head>  : ใช้อธิบายข้อมูลเกี่ยวกับเว็บ เช่น Title Author Keywords 


<body>...</body> : อธิบบายเนื้อหาหลักของเว็บ เช่น ใส่ข้อความต่างๆ รูปภาพ วิดิโอ คุณสมบัติต่างๆ(เช่น รูปพื้นหลัง , สีของตัวอักษร เป็นต้น)

กำหนดหัวเรื่อง(heading) -> <h1></h1> ถึง <h6></h6> : ตัวอักษรใหญ่ไปเล็ก

<a href="ใส่ลิ้งเว็บ...">.... </a>   // a = answer   // href = hyper reference   // สีฟ้า = attribute //สีน้ำเงินเข้ม = tag

ข้างใน <..> เรียกว่า attribute คือสามารถระบุคุณสมบัติต่างๆได้

<br/> : เว้นบรรทัด

<title>...</title>  : ชื่อเว็ปตรง tab web

html:5 -> พิมพ์ตอนเริ่มต้น โปรแกรมจะทำการ generate text ให้เลย 


<meta>  : การเข้า Character encoding(การเข้าถึงรหัสอักขระ)

<!--ข้อความอธิบาย-->  : เอาไว้ใช้อธิบายให้คนเขียนโค้ดคนอื่นรู้ได้ (ไม่ขึ้นหน้าweb)   -keyลัด- ctrl + /


<p>...</p>  :แสดงข้อมูลเป็น Paragrapghs จะเริ่มที่บรรทัดใหม่เสมอ

Tag ที่ใช้ร่วมกับ <p></p> : คั่นระหว่างข้างใน <p>...</p> ได้
เช่น
<small>...</small> : ตัวพิมพ์เล็ก 
<strong>...</strong> : ตัวหนา
<b>...</b>  : ตัวหนา
<i>...</i>  : ตัวเอียง
<u>...</u>  : ขีดเส้นใต้
<ins>...</ins> : ขีดเส้นใต้
<del>...</del>  : ขีดตัวอักษร
<mark>...</mark>  : Highlight ข้อความสีเหลือง
<sup>...</sup>  : เลขยกกำลัง  (บน)
<sub>...</sub> : ตัวห้อยเลข  (ล่าง)



<br/> : tag สำหรับขึ้นบรรทัดใหม่
<hr> : เส้นคั่นในแนวนอน

    <!-- internal => เชื่อมโยงweb page ในไฟล์เดียวกัน -->
    <!-- external => เชื่อมโยงweb ข้างนอก -->
    
<a href="page2.html" target="_blank" >page 2</a>   <!-- _blabk : ขึ้นtabใหม่ -->
<a href="page3.html" >page 3</a>        <!-- ทำงานใน tab เดียวกัน -->
<a href="shopping/shop.html" target="_blank" >SHOP</a>           <!-- within floder-->
<a href="../EP2.html" >กลับหน้าแรก</a>  <!-- ../ คืออกจากโฟลเดอร์ที่อยู่-->



tag รูปภาพ
<!-- internal -->
<p>
Lorem ipsum, dolor sit amet consectetur adipisicing elit. Et atque voluptates illo?
<br>   
<img src="img/OW1.png" alt="OW NOOB" width="120px" height="120px">     <!-- alt คือคำอธิบายรูปภาพ-->
</p>
<p>GAME OW</p>
<a href="page3.html" target="_blank">
    <img src="img/OW2.png" alt="OW GOOD" width="120px" height="120px">
</a>
<br>
<!-- external -->
<img src="https://i.natgeofe.com/n/4f5aaece-3300-41a4-b2a8-ed2708a0a27c/domestic-dog_thumb_square.jpg" alt="" width="120px" height="120px">


แสดงLists
- ใช้ตัวเลข (OL : Order List) : เรียงลำดับแบบย่อย
- ใช้สัญลักษณ์ (UL : Unorder Lists) : ไม่เรียงลำดับ

<ol type="รูปแบบการแสดงผล">       
    <li>...<li>
</ol>         

    ในtype
        * A =ตัวพิมพ์ใหญ่
        * a = ตัวพิมพ์เล็ก
        * I = เลขโลมันตัวใหญ่
        * i = เลขโลมันตัวเล็ก

<ul type="รูปแบบการแสดงผล">
    <li>...<li>
</ul>

    ในtype
        * disc - จุดสีดำ
        * circle - จุดวงกลมโปร่ง
        * square - สี่เหลี่ยมทึบดำ (ตัวเล็กทั้งหมด)


การสร้างตาราง(Table)
    <table>...</table> : กำหนดการสร้างตาราง
        <thead>...</thead> : กำหนดกลุ่มเนื้อหาส่วนหัวตาราง
            <th>...</th> : กำหนด column ที่แสดงผลในส่วนหัวของตาราง
                <tbody>...</tbody> : กำหนดกลุ่มเนื้อหาในตาราง
                <tfoot>...</tfoot> : กำหนดกลุ่มส่วนใต้ตาราง
                <tr>...</tr> : กำหนด rows ในตาราง
                    <td>...</td> : กำหนด columns

    *attributeของตาราง
        border="" : กำหนดความหนาของเส้นของตาราง
        width="%"  : กำหนดความกว้างเป็น%
        bgcolor="สี" : กำหนดสีพื้นหลังในตาราง
        <table bgcolor="สี"> : กำหนดสีrow และ column
        <tr bgcolor="สี"> : สี rows
        <td bgcolor="สี"> : สี coulmns

    colspan="x" : รวมcolumns ค่า x (ช่อง<td>)
    rowspan="x" : รวมแถว ค่า x คือจำนวนแถวที่ต้องการรวมเข้าด้วยกัน (ช่อง<tr>)
    align="left , center , right" : จัดตำแหน่งของภาพ หรืออักษรภายในช่องตาราง<td>
    ค่าปกติคือ left
    Cellpadding : ขยายพื้นที่จากตัวด้านในตาราง (หน่วย Pixel)
    
    Cellspacing : กำหนดขนาดเส้นตาราง ขยายพื้นที่ด้านนอก (หน่วย Pixel)

การจัดกลุ่มด้วย div , span
    <span>...</span> : จัดกลุ่มข้อความหรือtahต่างๆเข้าเป็นกลุ่มเดียวกันเพื่อกำหนด สี รูปแบบตัวอักษร หรือstyleให้กับข้อความ (inline :อ้างอิงพื้นที่ตามเนื้อหา)
    <div>...</div> : แบบเดียวกันกับ span แต่จะมีการขึ้นบรรทัดใหม่ก่อนเสมอ (Block :อ้างอิงพื้นที่โดยกำหนดให้เต็มพื้นที่ )

เขียน <style> ในส่วนของ <head>

<!-- solid คือสีทึบ-->

ิborder : ขนาด(px),เส้นสีหนามั้ย(เช่น solid) ,สีขอบ  -->กรอบ

HTML FORM
<form>...<form> : ผู้ใช้งานสามารถป้อนข้อมูลต่างๆได้ แล้วนำข้อมูลนั้นที่ป้อนไปประมวลผลอีกที
    attribute : action="" คือตัวส่งข้อมูลไปทางฝั่ง server พิมพ์ข้างใน<form>
    <input> : รับข้อความต่างๆ
        กำหนด type="" ข้างใน เพื่อระบุการกรอก เช่น text(ใส่ข้อความ)
    <select> : ตัวเลือกในรูปแบบ Drop-down
         <option> : สร้างตัวเลือก (ภายใน Drop-down ของ <select>)
            <!-- selected : คือตัวเลือกเริ่มต้น (พิมพ์ใส่ใน<option>)--> 
    <button> : สร้างปุ่ม
    <label> : กำหนดป้ายชื่อให้ช่องรับข้อมูล
    <textarea> : รับข้อความแบบหลายบรรทัดได้

ปุ่มส่งข้อมูลไปทางฝั่ง server 
    ใช้ type="submit"


Block : ความยาวเต็มบรรทัด
    <address>
    <article>
    <blockquote>
    <canvas>
    <dd>
    <div>
    <dl>
    <table>
    <dt>
    <fieldset>
    <fieldset>
    <figcaption>
    <figure>
    <footer>
    <form>
    <h1>-<h6>
    <header>
    <tfoot>
    <hr>
    <li>
    <main>
    <nav>
    <noscript>
    <ol>
    <p>
    <pre>
    <section>
    <tfoot>
    <ul>
    <video>
Inline : ความกว้างเท่ากับข้อความที่แสดง
    <a>
    <abbr>
    <acronym>
    <b>
    <bdo>
    <big>
    <br>
    <button>
    <cite>
    <code>
    <dfn>
    <em>
    <i>
    <img>
    <input>
    <kbd>
    <label>
    <map>
    <object>
    <output>
    <q>
    <samp>
    <script>
    <select>
    <small>
    <span>
    <strong>
    <sub>
    <sup>
    <textarea>
    <time>
    <tt>
    <var>



Class : กำหนดค่า attribute ใส่ซ้ำได้
ID : กำหนดรหัสเฉพาะด้วยการกำหนดค่า attribute   ไม่สามารถตั้งซ้ำได้

Semantic Tag : นำมาใช้แทน div หลายๆชั้น (ช่วยให้โครงสร้าง html มีความชัดเจนมากขึ้น)
    โครงสร้าง html ประกอบด้วย
        header (ส่วนหัว)                      
        <nav> (เมนูเว็บ หรือ ลิ้งไปเว็บอื่นๆ)                content เรียกว่า <main> (เนื้อหาหลัก) ประกอบด้วย <article>
        <article> ( ส่วนที่แสดงเนื้อหาของเว็บ ) 
        <section> ( กลุ่มหัวข้อย่อย)  ประกอบด้วย <article>
        <aside> (เนื้อหาอื่นๆที่แยกออกจากเนื้อหาหลัก ใช้แทนnavได้)
        <footer> (ส่วนท้าย)


Character Entity (สัญลักษณ์พิเศษ) 
    search ใน google เพื่อดูวิธีการพิมพ์ : https://html.spec.whatwg.org/multipage/named-characters.html
    
    เช่น &nbsp; (ช่องว่าง)
        &gt; (>)
        &lt; (<)
        &empty; (สัญลักษณ์ห้าม)
        &copy; (สัญลักษณ์ copyright : ลิขสิทธ์)
        &reg;  (เครื่องหมายการค้า)
        &yen; (สกุลเงินเยน)
        &pound; (สกุลเงินปอนด์)
        &euro; (สกุลเงินยูโร)


<code>...</code> : นำ source codeต่างๆ มาแสดงผลในหน้า web

<kbd>...</kbd> : สัญลักษณ์ keybord คีร์ลัดต่างๆการกดบนคีร์บอร์ด

<video> : แสดงวิดิโอบนหน้า web นำมาจากไฟล์ในเครื่อง   ( ระบุ control เพื่อควบคุมวิดิโอได้ )
    ระบุ <source src="ชื่อไฟล์" type="นามสกุลไฟล์">

<iframe> : แสดงวิดิโอบนหน้า web นำมาจากแหล่งอื่น แบบ external

<audio>...</audio> : นำไฟล์เสียงจากในเครื่อง มาแสดงบนหน้า web      ( ระบุ autoplay คือ เล่นอัตโนมัติ : ต้องเป็น browser ที่รองรับถึงทำได้)
    ระบุ <source src="ชื่อไฟล์" type="นามสกุลไฟล์">