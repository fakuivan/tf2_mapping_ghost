# tf2_mapping_ghost
A template for adding ghosts to your tf2 map

The ghost used on maps like koth_harvest_event is usually composed by:

<ul>
  <li><strong>func_train</strong></li>    
    <ul>
      <li><strong>trigger_stun</strong></li>
        <dd>the thing that scares you</dd>
      <li><strong>prop_dynamic</strong></li>
        <dd>the ghost model</dd>
      <li><strong>ambient_generic</strong></li>
        <dd>the boo! sound, triggered by the trigger_stun, usually delayed by .5s</dd>
      <li><strong>info_particle_system</strong></li>
        <dd>teleport efect</dd>
      <li><strong>path_trach</strong></li>
        <dd>a home track</dd>
      <li><em>some extras</em></li>
    </ul>
</ul>

To use the template you need to copy the contents of it into your map, create a track using the ``path_trach`` entity and add some triggers to teleport ``gTrain`` to the desired location. You need to trigger a ``StartForward`` on ``gTrain`` for it to start moving and for the teleport sounds and particles to show.
