# Object

```
const geometry = new THREE.BoxGeometry(1, 1, 1);
const material = new THREE.MeshBasicMaterial({ color: 0xff0000 });
const mesh = new THREE.Mesh(geometry, material);
scene.add(mesh);
```

# Position

```
//console.log(mesh.position.normalize());
//console.log(mesh.position.length());
// mesh.position.x = 0.7;
// mesh.position.y = 0.6;
// mesh.position.z = 1;
mesh.position.set(0.7, -0.6, 1);
```

# Scale

```
//mesh.scale.x = 2;
//mesh.scale.y = 0.5;
//mesh.scale.z = 0.5;
mesh.scale.set(2, 0.5, 0.5);
```

# Rotation

```
// Not object free. Rotation is a euler;
// Use Pi for half rotation = 3.14159
// Warning: Order of set axis is important (x -> y -> x)
mesh.rotation.reorder("YXZ");
mesh.rotation.x = Math.PI _0.25;
mesh.rotation.y = Math.PI_ 0.25;
```
