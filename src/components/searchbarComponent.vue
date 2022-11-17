<style lang="scss" scoped>
.search {
  // margin-top: 145px;
  display: flex;
  // margin-bottom: 145px;

  .searchbar {
    align-self: center;
    // width: 80%;
    height: 8vh;
    box-shadow: rgba(0, 0, 0, 0.35) 0px 5px 15px;
    border-radius: 6px;
    vertical-align: middle;
  }
  .row {
    margin-top: 17px;
  }
  .bt-text {
    padding: 10px 2px;
  }
  .btn-custom:hover {
    background-color: white;
    border: none;
  }
  .btn-custom:active {
    background-color: white;
    border: none;
  }
  .btn-custom {
    background-color: white;
    border: none;
  }
  .sicon {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    margin-top: 5px;
    i {
      padding-right: 4px;
      padding-left: 12px;
      margin-top: 5px;
    }
    #search {
      border: none;
      width: 100%;
    }
    #search:hover {
      border: none;
    }
    #search:active {
      border: none;
    }
    #search:focus {
      border: none;
    }
  }
}
</style>

<template>
  <div class="search">
    <div class="searchbar">
      <div class="row">
        <div class="col-5">
          <div class="sicon">
            <i class="fa fa-search" aria-hidden="true"></i>
            <input
              type="search"
              placeholder="Job title or keyword"
              name="job-type"
              id="search"
            />
          </div>
        </div>
        <div class="col-4">
          <div class="dropdown">
            <button
              class="btn btn-light dropdown-toggle btn-custom"
              data-bs-toggle="dropdown"
              aria-expanded="false"
            >
              <span class="bt-text"
                ><i
                  class="fa fa-map-marker"
                  aria-hidden="true"
                  style="padding-right: 4px"
                >
                </i
                >location
              </span>
            </button>
            <ul class="dropdown-menu dropdown-menu-light">
              <li><a class="dropdown-item active" href="#">Action</a></li>
              <li><a class="dropdown-item" href="#">Another action</a></li>
              <li><a class="dropdown-item" href="#">Something else here</a></li>
              <li><hr class="dropdown-divider" /></li>
              <li><a class="dropdown-item" href="#">Separated link</a></li>
            </ul>
          </div>
        </div>
        <div class="col-3">
          <button class="btn btn-primary" type="submit">Search</button>
        </div>
      </div>
    </div>
  </div>
</template>
