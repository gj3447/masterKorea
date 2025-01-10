<div>
  <input id="tab1" type="radio" name="tabs" checked>
  <label for="tab1">Tab 1</label>
  <input id="tab2" type="radio" name="tabs">
  <label for="tab2">Tab 2</label>
  <input id="tab3" type="radio" name="tabs">
  <label for="tab3">Tab 3</label>
  
  <div id="tab-content1" class="tab-content">
    <p>Content for Tab 1</p>
  </div>
  <div id="tab-content2" class="tab-content">
    <p>Content for Tab 2</p>
  </div>
  <div id="tab-content3" class="tab-content">
    <p>Content for Tab 3</p>
  </div>
</div>

<style>
  input[type="radio"] {
    display: none;
  }
  label {
    display: inline-block;
    padding: 10px 20px;
    margin-right: -1px;
    border: 1px solid #ccc;
    cursor: pointer;
    background: #f1f1f1;
  }
  input[type="radio"]:checked + label {
    background: white;
    border-bottom: 1px solid white;
  }
  .tab-content {
    display: none;
    padding: 20px;
    border: 1px solid #ccc;
    background: white;
  }
  input[type="radio"]:checked + label + .tab-content {
    display: block;
  }
</style>
