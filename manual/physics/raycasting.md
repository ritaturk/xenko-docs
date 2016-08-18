# Raycasting

Raycasting is the process of tracing along a vector (ray) to detect any intersection with colliders in a scene. This process can be used for instance to determine what object is under the mouse pointer when the user clicks somewhere in the 3D image.

Raycasting can be done in your code using the current ```Simulation``` object. Using the ```Simulation.Raycast(Vector3 from, Vector3 to)``` function, it is easy to check if any collider intersects with this ray, and retrieve the collider the ray first hits.

```cs
    simulation = this.GetSimulation();
    var result = simulation.Raycast(unprojectedNear, unprojectedFar);
    if (!result.Succeeded || result.Collider == null) return;

    var rigidBody = result.Collider as RigidbodyComponent;
    if (rigidBody == null) return;
```