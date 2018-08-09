wayang-hardware-dimension defines data which is intended primarily so that planning systems can render a simplified graphical view of physical devices comprising a hierachy of optional components, e.g. slots in a chassis.
For such an application a CAD file such as those described in ISO 10303 is considered too heavyweight, instead size is described as a simple cuboid which fully encloses the component. The origin of the component is the lower front left node of this cuboid. Where necessary the cuboid can be rotated in space around this origin. The vector from the origin of the parent to the origin of a child component is expressed in cartesian coordinates.
The result is that a device can report (or a file can contain):
1. Size and weight of a component instance 
2. The position and orientation of an installed component relative to the position of its parent component
3. Size and weight of a component type
4. The relative position and orientation of a component-class which is permenantly built into a parent component-type. This is included-child-offset-from-parent and included-child-orientation
            
