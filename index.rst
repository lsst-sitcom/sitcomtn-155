##################################################
Eyepiece Observations with the Auxiliary Telescope
##################################################

.. abstract::

   This Technote serves as a guide for performing eyepiece-based observations with the Auxiliary Telescope.

Introduction
============

.. note::
   **Eyepiece observations with the Auxiliary Telescope (AuxTel) require prior approval from SITCOM Management and XXXXXX.**

.. warning::
   Mandatory Personal Protective Equipment (PPE) required during eyepiece-based observations:

   #. Safety boots.
   #. Hard hat.
   #. High-visibility vest or jacket.
   #. Cold weather gear.
   #. Flashlight.

.. danger::
   This mode of observing with AuxTel requires personnel to be on the telescope floor while the telescope and dome are moving.
   The safety door interlock will have to be overridden.
   **Extreme caution is advised at all times.**

   **Collision hazard** with the telescope structure, dome, and telescope floor tables and equipment. **Please maintain a safe distance from the telescope mount.**

   **Fall hazard** on the telescope floor. **Please be aware of your surroundings while walking on the second floor of the telescope building, especially during nighttime.**

   **Entrapment hazard** with the telescope structure and dome. **Please maintain a safe distance from the telescope mount.**

   **Electrical hazard** with the dome slip-ring. **Please maintain a safe distance from the dome.**
   
Procedure - Starting Observations
=================================

#. **Prior authorization for AuxTel eyepiece observations from SITCOM management is mandatory.**

#. Ensure the mandatory PPE is worn before entering the AuxTel building.

#. Post a message in the Slack channels *summit-auxtel* and *summit-announce* communicating that you are about to start eyepiece-based observations with AuxTel.
   Additionally, inform the Observing Specialist (OS) on-duty about this.

#. Inside the AuxTel building, on the first floor, push the *Safety Gate Bypass* button on the ATMCS/Pneumatics (labeled AT Control Cabinet).
      
   .. figure:: ./_static/IMG_4687.JPG
      :width: 500px

   Figure 1: Safety Gate Bypass activation button.

#. Go to the Safety Gate, and press the *Release* button. A click sound will be heard, releasing the mechanism that allows the door to be opened.

   .. figure:: ./_static/IMG_4685.JPG
      :width: 500px    
 
   Figure 2: Safety Gate inside the first floor of the AuxTel building.   

#. Push the black handle of the door to the left, and then open the door.

#. Go up to the second floor. 
   **Please maintain a safe distance from the telescope and dome at all times, and especially when the telescope is moving.**

#. **Eyepiece installation:**
   The eyepiece is stored in its box inside Brian Stalder's locker, at the entrance of the main building. 
   **[We should identify a definitive storage location within AuxTel].**
   Remove the plastic cover from the Nasmyth port #1 black tube, and carefully insert the eyepiece into the slot.
   While holding the eyepiece with one hand, tighten the two screws between the tube and the eyepiece with the other, securing the eyepiece.
   
   .. figure:: ./_static/IMG_4688.JPG
      :width: 500px
 
   Figure 3: AuxTel Nasmyth Rotator port #1.

   **[Insert Picture of the eyepiece installed with the screws here.]**

#. **Tertiary mirror (M3) manual positioning:**
   The M3 motor is malfunctioning, and the positioning has to be made manually until the motor is replaced by the Electronics Group. 
   **2 people are needed for this procedure:**
   
   #. Identify the AT Pneumatics Box, beneath the telescope (see Figure 4 for reference), and open it using a screwdriver.
   #. Identify the M3 Indexer hose, and with the help of a screwdriver, depress the blue button highlighted in Figure 5.
   #. While one person holds the button depressed, the other one will have to manually rotate the M3 rotating table 180º (see Figure 6).
   #. Once the M3 is in position, the blue button in the AT Pneumatics Box can be un-pressed. 
   #. A slight manual adjustment will be needed in M3, until the piston gets inserted (producing a sound during the insertion).
      This is important, since once the piston is engaged, the rotary table will be locked.

   .. figure:: ./_static/IMG_4722.JPG
      :width: 500px

   Figure 4: AT Pneumatics Box.
   
   .. figure:: ./_static/IMG_4723.JPG
      :width: 500px
 
   Figure 5: Festo valve button to be depressed, highlighted with a red circle.

   .. figure:: ./_static/IMG_4724.JPG
      :width: 500px
 
   Figure 6: M3 rotating table.

#. Before moving the telescope and dome, carefully inspect that there are no objects or people in the way.

#. Initialize the AuxTel telescope, dome, and shutters.
   **[Consider adding instructions on how to operate AuxTel, or clarify that this task will be performed by experienced personnel or OS.]**

#. Slew to a target once all systems are ready for operations.

#. Once the telescope and dome are in position, you can begin observing with the eyepiece.
   A black and metallic step stool is available on the second floor, should it be needed to reach the eyepiece comfortably.
   
   .. figure:: ./_static/IMG_4756.JPG
      :width: 500px
 
   Figure 7: Step stool available in the second floor.

Procedure - Ending Observations and Closure
===========================================

#. Execute the *shutdown_all.py* script in the LOVE ScriptQueue. This script will park the telescope and dome.

#. Once the telescope and dome are parked, and the corresponding CSCs are in ``STANDBY``, the eyepiece can be removed.
   While holding the eyepiece with one hand, loosen the two screws and carefully remove the eyepiece. 
   Return the eyepiece to its box and store it inside Brian Stalder's locker. 
   **[We should identify a definitive storage location within AuxTel].**

#. **M3 manual positioning:**
   Do not forget to put the M3 back to LATISS, following the same procedure as in the previous section.

#. Go downstairs to the first floor. 

#. Close the Safety Gate, and pull the black handle to the right to lock it.

#. Press the lock button. A click sound will be heard, engaging the lock.

#. In the AT Control Cabinet, press the *Safety Gate Bypass* button to activate the Safety Gate Interlock.

#. Close the door of the AuxTel building on your way out.

#. Post a message in the Slack channels *summit-auxtel* and *summit-announce* communicating that you are done with the eyepiece observations with AuxTel, and inform the Observing Specialist (OS) on-duty about it.

*END OF THE PROCEDURE*