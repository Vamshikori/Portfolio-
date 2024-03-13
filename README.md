// Get form elements
const usernameInput = document.getElementById('username');
const passwordInput = document.getElementById('password');
const loginButton = document.getElementById('login-button');
const errorMessage = document.getElementById('error-message');

// Add event listener to the login button
loginButton.addEventListener('click', () => {
  // Reset error message
  errorMessage.textContent = '';

  // Check if username and password are empty
  if (usernameInput.value.trim() === '' || passwordInput.value.trim() === '') {
    errorMessage.textContent = 'Please enter your username and password.';
  }
});
