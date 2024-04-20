<template>
  <div class="d-flex justify-content-center">
    <b-row>
      <b-col cols="12" sm="12" md="12">
    <b-card class="mb-2 text-center">
      <b-card-text>
        <img 
        :src="$auth.user.picture"
        class="rounded-circle"
        style="width: 200px; height: 200px; object-fit: cover;"
        alt="Profile Image"
      >
        <h2>{{ $auth.user.name }}</h2>
        <p>{{ $auth.user.email }}</p>
      </b-card-text>

      <b-card>
        <b-card-text>
          <div>
            <pre>{{ JSON.stringify($auth.user, null, 2) }}</pre>
          </div>
        </b-card-text>
      </b-card>
    </b-card>
      </b-col>
    </b-row>
  </div>
</template>
