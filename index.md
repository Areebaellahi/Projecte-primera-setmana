<h2>Part 1 - el server que ens presten</h2>
<p> He creat un domini amb el meu nom i cognom areeba.ellahi.io</p>
<p> Després he creat un compte de correu amb aquell domini</p>
<p>aellahi@areebaellahi.io</p>
<p><img src="https://raw.githubusercontent.com/Areebaellahi/FOTOS/main/01.png" alt="Cat"></p>
<p> He enviat un email a joan@surfacad.edu i em dona un error de que aquest missatge no es pot arribar al destinatari perquè en un domini privat.</p> 
<p><img src="https://raw.githubusercontent.com/Areebaellahi/FOTOS/main/2.png"></p>
<p>Després he provat enviar un email al meu compte de l’institut i no em dona cap error i el missatge a arribat en la safata d’entrada.
</p>
<p><img src="https://raw.githubusercontent.com/Areebaellahi/FOTOS/main/3.png"></p>
<p><img src="https://raw.githubusercontent.com/Areebaellahi/FOTOS/main/1.png" alt="Cat"></p>
<h2>Part 2 - el nostre server</h2>
<p> En play with docker:</p>
<p> crearem un volum</p>
<p><img src="https://raw.githubusercontent.com/Areebaellahi/FOTOS/main/4.png" alt="Cat"></p>
<p>Després posem:</p>
<p>docker run \-p 443:443 \-e TZ=Europe/Andorra \-v volum_mail_server:/data \--name "areebaellahi.io" \-h "areebaellahi.io" \-t analogic/poste.io</p>
<p><img src="https://raw.githubusercontent.com/Areebaellahi/FOTOS/main/5.png" alt="Cat"></p>
<h2>Instalar Docker en la maquina inte:</h2>
<p>-sudo apt-get update</p>
<p>-sudo apt-get install apt-transport-https ca-certificates curl gnupg2 software-properties-common</p>
<p>-curl -fsSL https://download.docker.com/linux/debian/gpg | sudo apt-key add -</p>
<p>-sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/debian buster stable"</p>
<p>-sudo apt-get update</p>
<p>-sudo apt-get install docker-ce docker-ce-cli containerd.io</p>
<p>Ara ja tenim instalat el docker per comprovar el estat posem:</p>
<p>-sudo systemctl status docker</p>
<p><img src="" alt="Cat"></p>
<p>Un altre manera de provar si tenim instalat bé el docker posem docker run hello-word:</p>
<h2>Generació dels certificats:</h2>
<p>He decidit crear el certificat amb mkcert.</p>
<p>Per fer lo posem:</p>
<p>-sudo apt install libnss3-tools</p>
<p>-mkcert client.org</p>
<p>-mkcert server.org</p>
<p><img src="https://raw.githubusercontent.com/Areebaellahi/FOTOS/main/6.png" alt="Cat"></p>


