**Section 3: Describe features of computer vision workloads on Azure**.

This section focuses on how AI systems can "see" and interpret the visual world, and the powerful Azure services that enable these capabilities.

### Section 3: Features of Computer Vision Workloads on Azure

**What is Computer Vision (CV)?**

**Computer Vision (CV)** is a field of Artificial Intelligence that enables computers to derive meaningful information from digital images, videos, and other visual inputs. It's about teaching machines to "see" and understand the world in a way similar to humans.

The goal of computer vision is to automate tasks that the human visual system can perform, such as recognizing objects, faces, text, and even understanding scenes.

---

#### Key Computer Vision Tasks/Capabilities:

1.  **Image Classification:**

    - **Purpose:** Assigns a single category or label to an entire image. The model determines what the image _is_.
    - **Example:** Classifying an image as "cat," "dog," "landscape," or "building."
    - _Think of it as:_ Answering the question "What is in this picture (overall)?"

2.  **Object Detection:**

    - **Purpose:** Identifies the presence and _location_ of multiple objects within an image or video. It typically draws a "bounding box" around each detected object and labels it.
    - **Example:** In a photo of a street, identifying and drawing boxes around each "car," "pedestrian," and "traffic light."
    - _Think of it as:_ Answering "What objects are in this picture, and where exactly are they?"

3.  **Optical Character Recognition (OCR):**

    - **Purpose:** Extracts printed or handwritten text from images and converts it into machine-readable text.
    - **Example:** Scanning a document to convert it into an editable text file, reading text from a street sign in a photo, or extracting information from a receipt.
    - _Think of it as:_ Making text in images searchable and editable.

4.  **Facial Detection, Recognition, and Analysis:**

    - **Facial Detection:**
      - **Purpose:** Identifies the presence and location of human faces in an image or video. It simply tells you _if_ and _where_ a face is.
      - **Example:** A camera detecting that a face is present in its field of view.
    - **Facial Recognition:**
      - **Purpose:** Identifies a _specific individual_ by matching their face to a database of known faces.
      - **Example:** Unlocking your phone with your face, or identifying a known person in a security camera feed.
    - **Facial Analysis:**
      - **Purpose:** Extracts attributes or characteristics from a detected face.
      - **Example:** Determining a person's age, gender, emotion (smiling, sad), or head pose from their facial features.
    - _Think of it as:_ Detection (is there a face?), Recognition (whose face is it?), Analysis (what are the characteristics of this face?).

5.  **Semantic Segmentation:**
    - **Purpose:** This computer vision task involves classifying _every single pixel_ in an image as belonging to a particular class or object. Instead of just drawing a bounding box around an object, it creates a precise, pixel-level mask or outline of the object.
    - **Example:** In an image of a street, semantic segmentation would color every pixel belonging to a "car" in blue, every pixel belonging to a "road" in green, and every pixel belonging to a "pedestrian" in red, providing a very detailed map of the scene.
    - _Think of it as:_ Not just "where is the car?" but "exactly _which pixels_ make up the car?"

---

#### Relevant Azure Services for Computer Vision:

Microsoft Azure offers several powerful services that provide pre-built and customizable computer vision capabilities:

1.  **Azure AI Vision (formerly Computer Vision service):**

    - This is a general-purpose Cognitive Service that provides a wide range of pre-trained computer vision capabilities through APIs.
    - **Capabilities include:** Image analysis (tagging, describing images, identifying common objects), optical character recognition (OCR), and content moderation (detecting adult/racy content).
    - **Use Case:** When you need to analyze general images for common objects, scenes, or extract text without training a custom model.

2.  **Custom Vision:**

    - This service allows you to build, deploy, and improve your own custom image classification and object detection models.
    - **Use Case:** When the pre-trained Azure AI Vision models don't meet your specific needs (e.g., you need to identify very specific types of products, plant diseases, or unique machinery that the general model wouldn't know). You provide your own labeled images to train it.

3.  **Face service:**

    - A specialized Cognitive Service dedicated to facial detection, facial recognition (identifying individuals), and facial analysis (extracting attributes like emotion, age, gender).
    - **Use Case:** Applications requiring identity verification, emotion detection, or managing user profiles based on facial features.

4.  **Azure AI Document Intelligence (formerly Form Recognizer):**
    - While it uses advanced OCR, this service goes beyond simple text extraction. It's designed to understand the _structure_ of documents (like invoices, receipts, passports, or custom forms) and extract structured data (e.g., key-value pairs, tables).
    - **Use Case:** Automating data entry from forms, processing financial documents, or digitizing historical records with structured information.

- **Define Computer Vision**
- **For each key CV task (Image Classification, Object Detection, OCR, Facial Detection/Recognition/Analysis):**
  - Briefly describe its purpose.
  - Provide one new, distinct real-world example.
- **For each Azure CV Service (Azure AI Vision, Custom Vision, Face service, Azure AI Document Intelligence):**
  - Briefly state its primary purpose.
  - Provide one new, distinct real-world example of its use.
