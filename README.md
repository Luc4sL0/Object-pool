# What is Object Pool?
Object Pooling is an effective method for optimizing your projects and reducing the strain on the CPU caused by frequent creation and destruction of GameObjects. It's a recommended practice and design pattern to consider, as it helps to lighten the CPU load, allowing it to focus on more critical tasks instead of being overwhelmed by repetitive create and destroy operations.
# How this code works?
Firstly, it is important to highlight that there can only be one instance of the "ObjectPooler_manager" code in the scene.

By adding the code "ObjectPooler_manager.cs" to the scene, it will be possible to configure as many objects as necessary. Each added object needs a prefab (object saved on disk), a tag and a maximum number of distinct instances of it that can exist.

If you are interested in executing a set of operations when a certain object is reactivated by the Object pool, you can implement the interface present in the "IPooledObject.cs" code in your object's code to have access to the "OnObjectSpawn()" function.
