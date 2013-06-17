pointcloud_compress
===================

Compression/Decompression nodes for ROS pointclouds

Run a pointcloud_compress node on the machine which has the camera:

  <!-- Compressor -->
  <node pkg="pointcloud_compress" type="compress.py" name="compressor">
      <rosparam>
        input: /camera/depth/points2_pass_zyx
        hz: 5
      </rosparam>
  </node>


Run a pointcloud_decompress on a machine on a wired network machine
     
  <!-- Decompressor -->
  <node pkg="pointcloud_compress" type="decompress.py" name="decompressor" />
