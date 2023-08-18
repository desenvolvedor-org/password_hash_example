# password_hash_example

//faz a encodify
``
$options = ['cost' => 12,];
$password = "admin";
$password_encode = password_hash($password, PASSWORD_BCRYPT, $options);
``


//agora ele verifica se a senha é valida
``

if (password_verify($password, $password_encode)) {
    echo 'Password is valid!';
} else {
    echo 'Invalid password.';
}

``
