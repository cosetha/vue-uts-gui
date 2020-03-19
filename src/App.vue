<template>
  <b-container fluid class="m-0 p-0">
    <b-row class="m-0 p-0">
      <b-col cols="2" id="sidebar-wrapper" class="sticky-top vh-100">
        <b-row class="m-0 p-0 h-30">
          <div class="border-0 shadow bg-dark">
            <img
              src="https://source.unsplash.com/TMgQMXoglsM/50 0x350"
              class="card-img-top rounded-circle"
              alt="..."
            />
            <div class="card-body text-center">
              <h5 class="card-title text-white mb-0">Team Member</h5>
              <div class="card-text text-white-50">Web Developer</div>
            </div>
          </div>
        </b-row>
        <b-row class="m-0 p-0 h-50">
          <div class="side-content">
            <ul>
              <a href="#">Content</a>
              <div class="progress">
                <div
                  class="progress-bar progress-bar-striped bg-danger"
                  role="progressbar"
                  style="width: 100%"
                  aria-valuenow="100"
                  aria-valuemin="0"
                  aria-valuemax="100"
                ></div>
              </div>
              <a href="#">Content</a>
              <div class="progress">
                <div
                  class="progress-bar progress-bar-striped bg-info"
                  role="progressbar"
                  style="width: 50%"
                  aria-valuenow="50"
                  aria-valuemin="0"
                  aria-valuemax="100"
                ></div>
              </div>
              <a href="#">Content</a>
              <div class="progress">
                <div
                  class="progress-bar progress-bar-striped bg-warning"
                  role="progressbar"
                  style="width: 75%"
                  aria-valuenow="75"
                  aria-valuemin="0"
                  aria-valuemax="100"
                ></div>
              </div>
            </ul>
          </div>
        </b-row>
        <b-row class="m-0 p-0 h-25">
          <div class="border-0 shadow bg-dark w-100">
            <div class="card-body text-center">
              <h5 class="card-title text-white mb-0">Team Member</h5>
              <div class="card-text text-white-50">Web Developer</div>
            </div>
            <div class="card-body text-center">
              <h5 class="card-title text-white mb-0">Team Member</h5>
              <div class="card-text text-white-50">Web Developer</div>
            </div>
          </div>
        </b-row>
      </b-col>
      <b-col cols="10" class="m-0 p-0">
        <b-navbar toggleable="lg" type="dark" variant="dark" sticky="top">
          <b-navbar-brand to="/">NavBar</b-navbar-brand>
          <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
          <b-collapse id="nav-collapse" is-nav>
            <b-navbar-nav>
              <b-nav-item to="/">Home</b-nav-item>
              <b-nav-item to="about">About</b-nav-item>
            </b-navbar-nav>
          </b-collapse>
        </b-navbar>
        <router-view />
      </b-col>
    </b-row>
  </b-container>
</template>
<style>
* {
  margin: 0;
  padding: 0;
}

#sidebar-wrapper {
  background-color: #cccccc;
  margin: 0;
  padding: 0;
}

.side-content {
  width: 100%;
  z-index: 1;
  top: 0;
  left: 0;
  background-color: #111;
  opacity: 0.9;
  overflow-x: hidden;
  padding-top: 60px;
  transition: 0.5s;
}
.side-content ul {
  margin: 8px 0 0 0;
  list-style: none;
}
.side-content a {
  padding: 10px 10px 10px 30px;
  text-decoration: none;
  font-size: 22px;
  color: #ccc;
  display: block;
  transition: 0.3s;
}

.side-content a:hover {
  color: #fff;
}
</style>
