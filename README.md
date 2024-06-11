# VAGRANT

## Comandos para Vagrant

- `vagrant init box_name` -> Lee el Vagrantfile.
- `vagrant up` -> Crear la VM.
- `vagrant ssh` -> Para login.
- `vagrant reload` -> Actualizar la VM con el Vagrantfile.
- `vagrant halt` -> Para apagar.
- `vagrant destroy` -> Para destruir.
- `vagrant global-status –prune` -> Ver el estado de todas las máquinas.

## Para empezar:

1. Crear una carpeta donde se alojará la ISO.
2. Buscar la ISO en el cloud: [Vagrant Cloud - Laravel Homestead](https://app.vagrantup.com/laravel/boxes/homestead)
3. Copiar el nombre de la ISO.

### Pasos:

1. Inicializar el Vagrantfile:

    ```bash
    vagrant init nombre_iso
    ```

    Esto creará el `Vagrantfile`.

2. Iniciar la máquina virtual:

    ```bash
    vagrant up
    ```

    Empezará a descargar los archivos necesarios de la nube a tu ordenador.

3. Comprobar que la máquina se ha creado correctamente:

    ```bash
    vagrant box list
    ```

4. Verificar el estado de la máquina:

    ```bash
    vagrant status
    ```

    Esto te permitirá saber si está en ejecución y dónde.

5. Abrir VirtualBox y verificar que aparece la máquina virtual.

6. Acceder a la máquina virtual:

    ```bash
    vagrant ssh
    ```

### Para apagar y comprobar el estado:

1. Apagar la máquina virtual:

    ```bash
    vagrant halt
    ```

2. Verificar que la máquina está apagada:

    ```bash
    vagrant status
    ```
