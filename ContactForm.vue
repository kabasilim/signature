te>
  <form @submit.prevent="submitForm">
    <label for="name">Name:</label>
    <input type="text" id="name" v-model="formData.name" required>

    <label for="email">Email:</label>
    <input type="email" id="email" v-model="formData.email" required>

    <label for="message">Message:</label>
    <textarea id="message" v-model

