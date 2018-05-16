# BTVN_C3
<!DOCTYPE html>
<html lang="en">
<head>
<title>BTVN_C3</title>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
* {
    box-sizing: border-box;
}
body {
  margin: 0;
}
.header {
    background-color: #2528be4d;
    padding: 20px;
    text-align: center;
}
.topnav {
    overflow: hidden;
    background-color: #333;
}
.topnav a {
    float: left;
    display: block;
    color: #f2f2f2;
    text-align: center;
    padding: 14px 16px;
    text-decoration: none;
}
.topnav a:hover {
    background-color: #ddd;
    color: black;
}
.column {
    float: left;
    width: 33.33%;
    padding: 15px;
}
.row:after {
    content: "";
    display: table;
    clear: both;
}
.column {
    width: 100%;
}

</style>
</head>
<body>

<div class="header">
    <img src="https://www.developpez.net/forums/attachments/p358946d1/a/a/a" style="
    width: 800px;
    height: 200px;
">
</div>

<div class="topnav">
  <a href="#">Trang Chủ</a>
  <a href="#">Liên Hệ</a>
  <a href="#">Đăng Ký/Đăng nhập</a>
</div>

<div class="row">
  <div class="column">
  </div>
  </div>
 
<ul class="form-list">
    <li class="fields">
        <div class="customer-name">
<div class="field name-firstname">
<label for="firstname" class="required"><em>*</em>Tên</label>
<div class="input-box">
<input type="text" id="firstname" name="firstname" value="" title="Tên" placeholder="Tên" maxlength="255" class="input-text validate-alpha-spac required-entry" autocomplete="off">
</div>
</div>
<div class="field name-lastname">
<div class="input-box">
<input type="text" id="lastname" name="lastname" value="" title="Họ" placeholder="Họ" maxlength="255" class="input-text validate-alpha-spac required-entry" autocomplete="off">
</div>
</div>
</div>
    </li>
  <li class="fields"><label for="month" class="required"><em>*</em>Ngày sinh</label>
<div class="input-box customer-dob">
<div class="dob-day">
<select onchange="getElementById('day').value=this.value" autocomplete="off">
<option value="">Ngày</option><option value="01">01</option><option value="02">02</option><option value="03">03</option><option value="04">04</option><option value="05">05</option><option value="06">06</option><option value="07">07</option><option value="08">08</option><option value="09">09</option><option value="10">10</option><option value="11">11</option><option value="12">12</option><option value="13">13</option><option value="14">14</option><option value="15">15</option><option value="16">16</option><option value="17">17</option><option value="18">18</option><option value="19">19</option><option value="20">20</option><option value="21">21</option><option value="22">22</option><option value="23">23</option><option value="24">24</option><option value="25">25</option><option value="26">26</option><option value="27">27</option><option value="28">28</option><option value="29">29</option><option value="30">30</option><option value="31">31</option>					  
</select>
<input type="hidden" id="day" name="day" value="" title="Ngày" class="input-text validate-custom" autocomplete="off">
</div><div class="dob-month">
<select onchange="getElementById('month').value=this.value" autocomplete="off">
<option value="">Tháng</option><option value="01">01</option><option value="02">02</option><option value="03">03</option><option value="04">04</option><option value="05">05</option><option value="06">06</option><option value="07">07</option><option value="08">08</option><option value="09">09</option><option value="10">10</option><option value="11">11</option><option value="12">12</option>					
</select>
<input type="hidden" id="month" name="month" value="" title="Tháng" class="input-text validate-custom" autocomplete="off">
</div><div class="dob-year">
<select onchange="getElementById('year').value=this.value" autocomplete="off">
<option value="">Năm</option><option value="2006">2006</option><option value="2005">2005</option><option value="2004">2004</option><option value="2003">2003</option><option value="2002">2002</option><option value="2001">2001</option><option value="2000">2000</option><option value="1999">1999</option><option value="1998">1998</option><option value="1997">1997</option><option value="1996">1996</option><option value="1995">1995</option><option value="1994">1994</option><option value="1993">1993</option><option value="1992">1992</option><option value="1991">1991</option><option value="1990">1990</option><option value="1989">1989</option><option value="1988">1988</option><option value="1987">1987</option><option value="1986">1986</option><option value="1985">1985</option><option value="1984">1984</option><option value="1983">1983</option><option value="1982">1982</option><option value="1981">1981</option><option value="1980">1980</option><option value="1979">1979</option><option value="1978">1978</option><option value="1977">1977</option><option value="1976">1976</option><option value="1975">1975</option><option value="1974">1974</option><option value="1973">1973</option><option value="1972">1972</option><option value="1971">1971</option><option value="1970">1970</option><option value="1969">1969</option><option value="1968">1968</option><option value="1967">1967</option><option value="1966">1966</option><option value="1965">1965</option><option value="1964">1964</option><option value="1963">1963</option><option value="1962">1962</option><option value="1961">1961</option><option value="1960">1960</option><option value="1959">1959</option><option value="1958">1958</option>
</select>
<input type="hidden" id="year" name="year" value="" title="Năm" class="input-text validate-custom" autocomplete="off">
</div>    <div class="dob-full" style="display:none;">
<input type="hidden" id="dob" name="dob" autocomplete="off">
</div>

<div class="validation-advice" style="display:none;"></div>
</div>
<script type="text/javascript">
//<![CDATA[
var customer_dob = new Varien.DOB('.customer-dob', true, '%d/%m/%Y');
//]]>
</script>
</li> <li>
<label for="email_address" class="required"><em>*</em>Địa chỉ email (Tên đăng nhập)</label>
  <div class="input-box"> 
  <input type="email" autocapitalize="off" autocorrect="off" spellcheck="false" name="email" id="email_address" value="" title="Địa chỉ email" class="input-text validate-email required-entry validate-no-html-tags" autocomplete="off">
   </div>
    </li>
    <li class="fields">
 <div class="field">
  <label for="password" class="required"><em>*</em>Mật khẩu</label>
   <div class="input-box">
   <input type="password" name="password" id="password" title="Mật khẩu" class="input-text required-entry validate-password" autocomplete="off">
   </div>
  </div>
    </li>
    <li class="fields">
       <label for="street_1" class="required"><em>*</em>Địa chỉ</label>
        <div class="input-box">
      <input type="text" name="street[]" value="N/A" title="Địa chỉ" id="street_1" class="input-text validate-no-html-tags  required-entry" autocomplete="off">
        </div>
    </li>
  <li class="control" style="display: none;">
        <div class="input-box">
      <input type="checkbox" name="is_subscribed" title="Tôi muốn nhận đề nghị qua email" value="1" id="is_subscribed" checked="checked" class="checkbox" autocomplete="off">
        </div>
        <label for="is_subscribed">Tôi muốn nhận đề nghị qua email</label>
    </li>
    <li><label for="gender" class="required"><em>*</em>Giới tính</label>
        <div class="input-box">
    <!--<input type="radio" name="gender" value="1">Male</input>-->
    <input type="radio" name="gender" value="1" checked="checked" autocomplete="off">Nam
    <!--<input type="radio" name="gender" value="2">Female</input>-->
   <input type="radio" name="gender" value="2" autocomplete="off">Nữ
      </div>
        </li>
        <li class="fields">												
    <div class="field">
     <label for="telephone" class="required"><em>*</em>Số điện thoại di động</label>
       <div class="input-box">
      <input type="tel" name="telephone" id="telephone" value="" title="Điện thoại" class="input-text required-entry validate-mobile  required-entry" autocomplete="off">
        </div>
       </div>
    </li>
  <li class="fields">
  <div class="field">
 <label for="confirmation" class="required"><em>*</em>Nhập lại mật khẩu</label>
   <div class="input-box">
   <input type="password" name="confirmation" title="Nhập lại mật khẩu" id="confirmation" class="input-text required-entry validate-cpassword" autocomplete="off">
    </div>
 </div>
</li>
    <button type="submit" class="btn btn-primary" id="signup_button" data-disable-with="Creating account…">Đăng ký</button>
  
   <p class="required account-create-required">* Phải nhập thông tin</p>
 </body>
 </html>
