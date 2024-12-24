# nav-input
# nav-input
// Функция проверки имени
export function isValidName(name) {
  if (typeof name !== 'string') {
    return false; 
  }
  
  const words = name.trim().split(' '); 
  if (words.length < 2) {
    return false; 
  }
  
  return words.every(word => word[0] === word[0].toUpperCase()); 
}


// Функция проверки пароля
export function isValidPassword(password) {
  if (typeof password !== 'string' || password.length < 8) {
    return false; 
  }
  
  const hasDigit = /\d/; 
  return hasDigit.test(password); 
}

