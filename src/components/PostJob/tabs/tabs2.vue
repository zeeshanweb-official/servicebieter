<template>
<div class="row">
    <div class="col-12">
        <div class="py-3">
            <slot name="tabs"></slot>

  <!-- Tab panes -->
  <div class="tab-content">
    <slot name="details1"></slot>
    <slot name="details2"></slot>    
  </div>
</div>
    </div>
</div>
</template>
<style scoped>
.nav-tabs .nav-item.show .nav-link,
.nav-tabs .nav-link.active,
.nav-tabs .nav-link.active:hover {
  border-color: #495057 #495057 #fff;
}

.nav-tabs {
  border-bottom-color: #495057;
}

.nav-tabs {
     border-bottom: none !important;
}
.nav-tabs .nav-link:hover {
  background-color: #eee;
  
}
.nav-tabs .nav-link.active:hover{
  background-color: #eee;    
  border-top: 2px solid #bd2522;
  border-bottom: 2px solid #bd2522;
}
.nav-tabs .nav-link.active {
  background-color: transparent !important;
  border-top: 2px solid #bd2522;
  border-bottom: 2px solid #bd2522 !important;
  border-left: none;
  border-right: none;
  color: #9ac034 !important;
  border-radius: 0%;
  box-shadow:none !important;
}

.nav-tabs .nav-link {
  margin-right: 4px;
  background-color: #fafafa;
  color:#AAA;
  border-radius: 0%;
  padding: 10px;
  border: 1px solid #d4cfcf;
}

</style>