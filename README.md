StateProvider is a provider that exposes a way to modify its state. It is a simplification of StateNotifierProvider, designed to avoid having to write a StateNotifier class for very simple use-cases.

StateProvider exists primarily to allow the modification of simple variables by the User Interface.
The state of a StateProvider is typically one of:

an enum, such as a filter type
a String, typically the raw content of a text field
a boolean, for checkboxes
a number, for pagination or age form fields
You should not use StateProvider if:

your state needs validation logic
your state is a complex object (such as a custom class, a list/map, ...)
the logic for modifying your state is more advanced than a simple count++.
