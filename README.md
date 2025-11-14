# CPU Architecture Playground (in-progress)

An interactive 3D educational platform for understanding CPU architecture through hands-on logic gate manipulation and circuit building.

<!-- ![CPU Playground Header]() -->
[Gate to Demo](https://0and1.vercel.app)

## Features

- **3D Interactive Canvas**: Drag and drop logic gates in a fully interactive 3D environment
- **7 Logic Gates**: AND, OR, NOT, NAND, NOR, XOR, and XNOR gates
- **Visual Connections**: Create wire connections between gates with visual signal flow
- **Live Testing**: Test circuits in real-time with interactive input toggles
- **Multiple Playgrounds**: Work on different circuits simultaneously with tabbed workspaces
- **Dark/Light Mode**: Comfortable viewing in any environment
- **Predefined Examples**: Learn from pre-built CPU components like Full Adders and SR Latches
- **Fully Responsive**: Works on desktop, tablet, and mobile devices

## How to Use

### 1. Adding Logic Gates

Click on any gate in the **Gate Library** (left sidebar) to add it to the 3D canvas:

- **AND Gate**: Outputs true only when both inputs are true
- **OR Gate**: Outputs true when at least one input is true
- **NOT Gate**: Inverts the input signal (single input)
- **NAND Gate**: NOT-AND - opposite of AND gate
- **NOR Gate**: NOT-OR - opposite of OR gate
- **XOR Gate**: Outputs true when inputs are different
- **XNOR Gate**: Outputs true when inputs are the same

<!-- ![Gate Library and Truth Tables](/images/screenshot-20-28174-29.png) -->

### 2. Moving Gates in 3D Space

**Drag Gates:**
- Click and hold on any gate
- Move your mouse to drag it across the grid plane
- Release to place the gate
- The cursor changes to a grab icon when hovering over gates

**Camera Controls:**
- **Rotate**: Click and drag on empty space
- **Zoom**: Use mouse wheel to zoom in/out
- **Reset View**: Rotate to find the best angle for your circuit

### 3. Connecting Gates

**Creating Connections:**
1. Click on an **output port** (the sphere on the right side of a gate)
2. Click on an **input port** (spheres on the left side of another gate)
3. A wire connection will be created between them

**Connection Colors:**
- **Green**: Active signal (logic HIGH/1)
- **Gray**: Inactive signal (logic LOW/0)
- **Cyan** (when hovering): Available for connection

**Removing Connections:**
- Select a gate in the Test Panel
- Delete the gate to remove all its connections
- Or clear the entire canvas using the "Clear Canvas" button

### 4. Testing Your Circuit

**Test Panel** (right sidebar):

1. **Select a Gate**: Click on any gate in the 3D canvas
2. **View Gate Info**: See the gate type and its truth table
3. **Toggle Inputs**: Use the switches to change input values (0 or 1)
4. **Watch Output**: The output updates in real-time based on gate logic
5. **Signal Propagation**: Connected gates automatically receive signals

**Real-Time Features:**
- Input changes immediately affect gate outputs
- Signals propagate through connected gates automatically
- Visual feedback shows active/inactive states

### 5. Multiple Playgrounds

**Working with Tabs:**
- Click **"New Circuit"** to create a new playground
- Switch between playgrounds using the tabs at the top
- Each playground maintains its own gates and connections
- Close tabs with the X button (except the last one)

**Pre-Built Examples:**
- **Half Adder Demo**: Simple addition circuit
- **Full Adder**: Complete 1-bit adder (CPU building block)
- **SR Latch**: Basic memory cell demonstration

These examples show how basic gates combine to create CPU components.

## Building CPU Components

### Example: Full Adder Circuit

A Full Adder is a fundamental CPU component that adds two bits plus a carry bit:

**Inputs:**
- A: First bit
- B: Second bit
- Cin: Carry in

**Outputs:**
- Sum: Result of A + B + Cin
- Cout: Carry out

**Circuit Construction:**
1. Two XOR gates for sum calculation
2. Two AND gates for carry detection
3. One OR gate for final carry output

This demonstrates how complex CPU operations are built from simple logic gates.

### Example: SR Latch (Memory)

An SR Latch is a basic memory cell that can store 1 bit:

**Components:**
- Two NOR gates with feedback loops
- Set (S) and Reset (R) inputs
- Q and Q' (not Q) outputs

This shows how CPUs store data using logic gates.

## Learning Path

1. **Start Simple**: Experiment with single gates and their truth tables
2. **Create Combinations**: Connect two gates (e.g., AND + NOT = NAND)
3. **Build Half Adder**: Use the pre-built example to understand addition
4. **Construct Full Adder**: Build from scratch using the example as reference
5. **Create Memory**: Build an SR Latch to understand data storage
6. **Complex Circuits**: Combine multiple components into larger systems

## Tips and Best Practices

- **Organize Your Circuit**: Arrange gates in logical groups (inputs on left, outputs on right)
- **Use Multiple Playgrounds**: Separate complex circuits into multiple tabs
- **Test Frequently**: Verify each connection works before adding more gates
- **Study Examples**: Learn from the pre-built circuits before building your own
- **Color Coding**: Watch the wire colors to understand signal flow
- **Start Small**: Build simple circuits before attempting complex CPU components

## Keyboard Shortcuts

- **Delete Selected Gate**: Press Delete or Backspace
- **Clear Canvas**: Use the "Clear Canvas" button in header
- **Zoom**: Mouse wheel
- **Rotate View**: Click and drag on empty space

## Troubleshooting

**Gates won't move:**
- Make sure you're clicking and dragging on the gate itself
- Camera controls may interfere - try clicking directly on the gate mesh

**Can't create connections:**
- Ensure you click output port first, then input port
- Or click input port first, then output port
- You cannot connect gates to themselves

## Contributing

Contributions are welcome once goes public This is an educational tool designed to help students and enthusiasts understand CPU architecture.
