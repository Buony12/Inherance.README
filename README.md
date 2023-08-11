# Inherance.README
# Define a class called Square
class Square:
  """This is a class that defines a square by its size

  Attributes:
    size (int): The size of the square
  """

  # Define a constructor method that takes an optional size parameter
  def __init__(self, size=0):
    """This is a method that initializes the instance attribute size

    Args:
      size (int, optional): The size of the square. Defaults to 0.

    Raises:
      TypeError: If size is not an integer
      ValueError: If size is less than 0
    """
    # Check if size is an integer
    if type(size) is not int:
      # Raise a TypeError exception with the message "size must be an integer"
      raise TypeError("size must be an integer")
    # Check if size is less than 0
    if size < 0:
      # Raise a ValueError exception with the message "size must be >= 0"
      raise ValueError("size must be >= 0")
    # Assign the size parameter to the instance attribute size
    self.size = size
