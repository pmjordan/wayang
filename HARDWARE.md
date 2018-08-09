wayang-hardware.yang extends RFC 8348 so that devices can :
1) Report on the component types (i.e. classes or specifications of components) which may be added to components that already comprise the device. This is the permitted-child-type list.
2) Provide a list of component types which can be referenced by the function 1. above. This is the component-type list.
3) Report on the component-types which are permenantly built into the component-types listed in function 2. above. This are primarily components of type slot, otherwise known as holders. This is the includes-child-type list.

It is recognised that device instance software may not have the ability to support these features immediately but a similar, machine readable data file direct from the equipment vendor would be a useful first step. Such a file would not have any entries in the component list which causes issues when parsing the file. These can be resolved if such files are marked as such using the presentation attribute.