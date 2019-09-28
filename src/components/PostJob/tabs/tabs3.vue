<template>
    <div>
        <div class="card-header custext p-1" style="font-size:21px;">Select Inquir Type</div>
        <div class="card-body">
          <div class="py-3">
            <div class="row">
              <div class="col-3"></div>
              <div class="text-center">
                <ul class="nav nav-tabs tablist2" role="tablist">
    <li class="ml-2">&nbsp;</li>
    <li class="nav-item newnavitem">
      <a class="nav-link newnavlink " data-toggle="tab" href="#home3" role="tab"><i class="fa fa-pencil-square-o"></i> Assignment </a>
    </li>
    <li class="nav-item newnavitem">
      <a class="nav-link newnavlink" data-toggle="tab" href="#profile3" role="tab"><i class="fa fa-money"></i> Cost Estimated</a>
    </li>
    <li class="nav-item newnavitem">
      <a class="nav-link newnavlink" data-toggle="tab" href="#messages4" role="tab"><i class="fa fa-bullhorn "></i> Offer</a>
    </li>
  </ul>

  <!-- Tab panes -->
  <div class="tab-content">
    <div class="tab-pane p-2" id="home3" role="tabpanel"></div>
    <div class="tab-pane p-2" id="profile3" role="tabpanel"></div>
    <div class="tab-pane p-2" id="messages4" role="tabpanel"><div class="py-3">
  <ul class="nav nav-tabs tablist2" role="tablist ">
    <li class="ml-3"></li>
    <li class="nav-item newnavitem">
      <a class="nav-link newnavlink active" data-toggle="tab" href="#none" role="tab"><i class="fa fa-file-text-o "></i>Verbindlich</a>
    </li>
    <li class="nav-item newnavitem">
      <a class="nav-link newnavlink" data-toggle="tab" href="#newhome" role="tab"><i class="fa fa-edit "></i>Unverbindlich</a>
    </li>
    <li class="nav-item newnavitem">
      <a class="nav-link newnavlink" data-toggle="tab" href="#newmessages" role="tab"><i class="fa fa-window-restore "></i>Both</a>
    </li>
  </ul>

  <!-- Tab panes -->
</div>
</div>
  </div>
              </div>
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

.nav-tabs .nav-link:hover {
  background-color: #eee;
  
}
.nav-tabs .nav-link.active:hover{
  background-color: #eee;    
  border-top: 2px solid #bd2522;
  border-bottom: 2px solid #bd2522;
}
.nav-tabs .nav-link.active {
  background-color: transparent;
  border-top: 2px solid #bd2522;
  border-bottom: 2px solid #bd2522;
  border-left: none;
  border-right: none;
  color: #9ac034;
  border-radius: 0%;
}

.nav-tabs .nav-link {
  margin-right: 4px;
  background-color: #fafafa;
  color:#AAA;
  border-radius: 0%;
  padding: 10px;
  border: 1px solid #d4cfcf;
}

/* Not essential */
.tablist2{
  border-bottom:none !important;
}

</style>