# Robotic Gripper Arm

## The main idea

This project is centered on the end effector: a two-finger gripper carried by an articulated arm. The blue gear pair and pale connecting links are the key visual clues. They indicate a synchronized mechanism intended to make both fingers open and close together around an object.

Unlike the other folders, this one separates the complete robot from the gripper subassembly. That makes it suitable for developing the hand in isolation while still showing how it mounts to the wrist.

## Two assembly entry points

Use `fully assembled robotic arm.SLDASM` when the goal is to understand the robot's overall reach and the gripper's position at the end of the chain. Use `gripper arm.SLDASM` when the goal is to inspect the finger pivots, gears, drive housing, links, and circular mounting interface.

The remaining files, `Part1.SLDPRT` through `Part11.SLDPRT`, are the individual SolidWorks parts that make up these assemblies.

## Mechanism tour

![Full robot with open gripper](<Screenshot (86).png>)

The complete assembly shows the gripper installed on the wrist. The yellow main link and red upper arm carry the tool, while the blue gear components sit at the hand where the closing motion is organized.

![Side profile of the arm](<Screenshot (87).png>)

This side profile clarifies the approach direction of the fingers and the sequence of arm joints leading to them. It is the most useful pose for thinking about how the hand reaches an object.

![Gripper mechanism from above](<Screenshot (88).png>)

The overhead view isolates the hand's moving parts and its attachment to the arm. The paired gears and short links are especially visible here, making this screenshot the natural starting point for a gripper motion study.

## What remains to be defined

The CAD geometry does not by itself specify finger travel, gear ratio, grip force, payload, actuator choice, materials, or guarding. Those values, along with mate behavior and interference checks, should be validated before fabrication or operation.
