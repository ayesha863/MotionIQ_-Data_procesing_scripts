Here’s a clearer and more polished version of your guide to the data preprocessing scripts:

---

## 📁 Data Preprocessing Scripts Guide

This document provides a complete overview of the preprocessing scripts and notebooks used in the dataset pipeline.

---

### 🔧 Script Descriptions

**1. `Count`**
Counts the total number of rows in all files within the dataset.

**2. `Hierarchy Viewer`**
Displays the folder structure to help visualize the dataset’s hierarchy.

**3. `Plot Sensor Data`**
Plots sensor data from a single file for inspection.

**4. `Plot Graphs with Dimension`**
Notebook for collectively visualizing sensory data across multiple files or dimensions.

**5. `Convert to Atomic`**
Converts 3-minute activity recordings into 5-second atomic events.

**6. `Delete Last Row`**
Removes the last (potentially incomplete) row from each file.

**7. `Final Fixed 4 Second`**
Notebook that converts event files into JSON format, ready for machine learning model input.

**8. `Structured Data Code`**
Reorganizes folder hierarchy from collection format to a structure compatible with JSON conversion.

**9. `Sync`**
Synchronizes sensor files based on aligned start and end times (late start, early finish).

**10. `Verify Data Timestamps`**
Checks that sensor file timestamps align with expected event times *before* syncing and restructuring.

**11. `Verify`**
Verifies duration and value consistency *before* syncing and restructuring.

**12. `Verify Timestamps Sync Data`**
Verifies timestamps *after* syncing and restructuring.

**13. `Verify Sync Data`**
Verifies duration and values *after* syncing and restructuring.

---

### 🧭 Recommended Script Execution Order

1. **Standardize Subject Names**
2. **Standardize Activity Names**
3. **Delete Last Row**
4. **Structured Data Code**
5. **Sync**
6. **Convert to Atomic**
7. **Final Fixed 4 Second (JSON Conversion)**

> ⚠️ *Note:* The remaining scripts are primarily used for verification. Each script accepts a path to the base folder containing the three device folders.

---

### 🏷️ Standard Activity Labels

* `bending`
* `walking`
* `standing_up_from_sitting`
* `sitting_down_from_standing`
* `slow_walk`
* `squatting`
* `open_door`
* `close_door`
* `quick_walk`
* `sitting`
* `put_on_floor`
* `pick_from_floor`
* `laying_down_from_sitting`
* `standing_up_from_laying`
* `typing`
* `jogging`
* `clean_the_table`
* `open_bag`
* `open_big_box`
* `reading`
* `close_lid_by_rotation`
* `plugin`
* `throw_out`
* `laying`
* `eat_small_things`
* `talk_using_phone`
* `standing`
* `upstairs`
* `downstairs`
* `drink_water`
* `fall_forward`
* `fall_right`
* `fall_backward`
* `fall_left`
* `fall_forward_when_trying_to_sit_down`
* `fall_backward_while_trying_to_sit_down`
* `fall_forward_while_trying_to_stand_up`
* `fall_backward_while_trying_to_stand_up`

---

### ⏱️ Three-Minute Activities

* `quick_walk`
* `jogging`
* `laying`
* `reading`
* `sitting`
* `slow_walk`
* `standing`
* `talk_using_phone`
* `typing`
* `walking`
* `clean_the_table`


