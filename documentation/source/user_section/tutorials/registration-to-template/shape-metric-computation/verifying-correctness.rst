.. _verifying-correctness:

Verifying the correctness of the metrics
****************************************

You may have noticed that the csv files generated by ``sct_process_segmentation`` also include the angles between the cord centerline and the normal to the axial plane. ``angle_AP`` corresponds to the angle about the AP axis, while ``angle_RL`` corresponds to the angle about the RL axis. These angles are used to correct for the tilt of the spinal cord relative to the superior-inferior axis. Therefore, if you obtain inconsistent CSA values, it is a good habit to verify that the values of these angles are reasonable.

.. figure:: https://raw.githubusercontent.com/spinalcordtoolbox/doc-figures/master/shape-metric-computation/csa-angles.png
   :align: center
   :figwidth: 80%

To demonstrate, below are the angles provided in the CSV file produced by :ref:`csa-perlevel`.

.. csv-table:: AP and RL angles produced in ``csa_perlevel.csv``
   :file: angle-ap-rl.csv
   :header-rows: 1